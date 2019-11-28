# Github-high-frequency-tips

## all git information were stored in .git/ directory, which is a hidden directory

git init     initialize git


git status   check the files that changed

### add files to git for tracking

git add -A   stages all changes

git add .    stages new files and modifications, without deletions

##### git add -all, git add . are the same in modern version of git.

git add -u   stages modifications and deletions, without new files

##### don't edit the file you have added to git. It would make up to be an unreachable file.

### commit git

git commit -m "comments"     commit git, comment should be accurate and wise.

##### git commit --allow-empty -m "nothing happened", you can do it with -allow-empty

##### 「工作目錄（Working Directory）」
git add .
##### 「暫存區（Staging Area）」
git commit -m "comment"
##### 「儲存庫（Repository）」

git commit -a -m "update content"    do add and commit in one command, but it won't apply the new files.

git log     check git logs

 -oneline     shrink information to one line
 
 --author="name"     find commits by author's name
 
 --author="Sherly\|Eddie"     find two name, separate by \ and | (or).

 -S "Ruby"    check for everything about "Ruby"

 --since="9am" --until="12am" --after="2017-01"     find commits in specific period.

##### The key is SHA-1（Secure Hash Algorithm 1）https://gitbook.tw/chapters/using-git/how-to-calculate-the-sha1-value.html


