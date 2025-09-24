# Challenge Name
implicit relative path

## My solve
**Flag:** `pwn.college{g0PeDXuakedCzQzLXRrGxog7KIN.QXxUTN0wSOyEzNzEzW}`

```bash
Connected!
hacker@paths~implicit-relative-path:~$ /challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ .challenge/run
bash: .challenge/run: No such file or directory
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{g0PeDXuakedCzQzLXRrGxog7KIN.QXxUTN0wSOyEzNzEzW}
```
## Incorrect tangents I went on
I wrote .challenge/run instead of ./run

## What I learned
I learned using . to access implicit relative paths

## References 
none

