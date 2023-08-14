# Introduction

## Basic concepts

### Diff

==Used to get difference between 2 files==

=='-' indicates deletions ==

=='+' indicates additions==

=='-u' is for unified format (+,-)==

To get diff use:
`diff -u old_file new_file`

![](Images&Links/Pasted%20image%2020230730221153.png)

### Diff file or Patch file

==This file shows the suggested changes==

To generate such file use:
`diff -u old_file new_file > change.diff`

Snip of patch file:
![](Images&Links/Pasted%20image%2020230730222020.png)
![](Images&Links/Pasted%20image%2020230730222059.png)

To apply patch file use:
`patch oldfile.py < change.diff`

==Entire directories can also be patched==




# Using GIT locally

## Advanced GIT interaction

### Skipping the staging area

 `git commit -a`   Shortcut to stage any changes to tracked files and commit them in one step 

*If the modified file has not been tracked we need to add it to repo first*

==GIT uses the Head alias (also can be thought of as a bookmark) to represent the currently checked out snapshot of the project==

![](Images&Links/Pasted%20image%2020230813130707.png)

### Getting more info about change

`git log -p`  Shows the log of changes along with the code changes , useful to check what change broke down the tool

To check individual commit use `git log` to get commits with commit ID , these commit ID can then be used to check code change using

`git show "COMMIT ID" `

To get stats such as no. for lines added or removed use `git log --stat`

To look at unstaged changes at any point used `git diff`

To get more info on changes being added use `git add -p`

To look at staged changes which have not been committed using `git diff --staged`



``
