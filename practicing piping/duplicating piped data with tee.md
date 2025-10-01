# Challenge Name
duplicating piped data with tee
## My solve
**Flag:** pwn.college{M85Oeec_t-U0YanRAOMqHpkKyrB.QXxITO0wSOyEzNzEzW}``

```bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ cat /challenge/pwn
#!/opt/pwn.college/bash

echo "Processing..." > /dev/tty
sleep 1
DIR=$(/bin/dirname ${BASH_SOURCE[0]})
if ! $DIR/chio.py --check_stdout_pipe tee 2>/dev/null && ! $DIR/chio.py --check_stdout_pipe challenge_shellscript 2>/dev/null
then
        fold -s <<< "You must pipe the output of /challenge/pwn into /challenge/college (or 'tee' for debugging)." > /dev/tty
        exit 1
fi

SECRET_VAL=$(tail -c+13 /flag | head -c8)
if [ "$1" != "--secret" ] || [ "$2" != "$SECRET_VAL" ]
then
        echo "Usage: $0 --secret [SECRET_ARG]"
        echo ""
        echo "SECRET_ARG should be \"$SECRET_VAL\""
        sleep 8
        exit 2
fi

echo "Correct! Passing secret value to /challenge/college..." > /dev/tty
echo "SUPERSECRET:$(tail -c+20 /flag | head -c4)"
sleep 8
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee /dev/tty | /challenge/college
Processing...
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "M85Oeec_"
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret M85Oeec_ | tee /de/tty | /challenge/college
Processing...
/bin/tee: /de/tty: No such file or directory
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{M85Oeec_t-U0YanRAOMqHpkKyrB.QXxITO0wSOyEzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
I learned how to duplicate piped data using tee command

## References 
none

