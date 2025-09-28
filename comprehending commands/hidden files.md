# Challenge Name
hidden files
## My solve
**Flag:** `pwn.college{QSSXyufFoAs5J-cvsmV4MQND-K4.QXwUDO0wSOyEzNzEzW}`

```bash
Connected!
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv          bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-104591231228  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-104591231228
pwn.college{QSSXyufFoAs5J-cvsmV4MQND-K4.QXwUDO0wSOyEzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
I learnt that we can't see files starting with . using ls command so we add -a to view it

## References 
none

