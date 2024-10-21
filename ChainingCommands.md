# Chaining with Semiconlons
Get the flag by using `/challenge/pwn;/challenge/college`

# Your First Shell Script
Used `echo "/challenge/pwn;/challenge/college">x.sh` to create the shell script and then ran the shell script by `bash x.sh` getting the flag

# Redirecting Script Output
Ran `echo "/challenge/pwn; /challenge/college" > x.sh` then piped it by `bash x.sh | /challenge/solve` to get the flag

# Execuatable Shell Scripts
Ran `echo "/challenge/solve">x.sh` then changed file permissions by  `chmod a+x x.sh` after which I executed the script by using `./x.sh` to get the flag
