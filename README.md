# Github-high-frequency-tips

## all git information were stored in .git/ directory, which is a hidden directory

### git only tracking files which means empty directory will be ignored.
### You can add .keep(empty file) file under the directory to make it tracked by git.

git init     Initialize git

git status   Check the files that changed


***
***
***

### add files to git for tracking

git add -A   Stages all changes

git add .    Stages new files and modifications, without deletions

##### git add -all, git add . are the same in modern version of git.

git add -u   Stages modifications and deletions, without new files

##### don't edit the file you have added to git. It would make up to be an unreachable file.

### commit git

git commit -m "comments"     Commit git, comment should be accurate and wise.

##### git commit --allow-empty -m "nothing happened"  You can do it with -allow-empty

### Brief
##### 「工作目錄（Working Directory）」
git add .
##### 「暫存區（Staging Area）」
git commit -m "comment"
##### 「儲存庫（Repository）」

git commit -a -m "update content"    Do add and commit in one command, but it won't apply the new files.

##### git commit -m -amend "comment"     Change the lastest commit comment by "-amend"

***
***
***

git log     Check git logs

 -oneline     Shrink information to one line
 
 --author="name"     Find commits by author's name
 
 --author="Sherly\|Eddie"     Find two name, separate by \ and | (or).

 -S "Ruby"    Check for everything about "Ruby"

 --since="9am" --until="12am" --after="2017-01"     Find commits in specific period.

##### The key is SHA-1（Secure Hash Algorithm 1）https://gitbook.tw/chapters/using-git/how-to-calculate-the-sha1-value.html

git rm welcome.html --cached With "--cached", it won't delete welcom.html, it make git no more track the file.

***
***
***


### Ignore files you don't want to be tracked.

##### touch .gitignore     Make a file name .gitingnore and edit the file for ignore rules.

##### ignore secret.yml
secret.yml

##### ignore config 目錄下的 database.yml
config/database.yml

##### 忽略所有 db 目錄下附檔名是 .sqlite3 的檔案
/db/*.sqlite3

##### 忽略所有附檔名是 .tmp 的檔案
*.tmp

##### 當然你要忽略自己也可以，只是通常不會這麼做
.gitignore

