# Challenge Name
helpful programs
## My solve
**Flag:** `pwn.college{AqaF2rjyQ1NL9JEN7KOnVhMgePN.QX3IDO0wSOyEzNzEzW}`

```bash
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 219
hacker@man~helpful-programs:~$ /challenge/challenge -g 219
Correct usage! Your flag: pwn.college{AqaF2rjyQ1NL9JEN7KOnVhMgePN.QX3IDO0wSOyEzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
I learned how to invoke programs which don't have a manpage using a special argument called --help

## References 
none

