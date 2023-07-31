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


