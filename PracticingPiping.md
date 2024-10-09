# Redirecting output
`echo PWN > COLLEGE` to get the flag.

# Redirecting more output
Use `/challenge/run > myflag` and then `cat myflag` to get the flag.

# Appending output
Use  `/challenge/run >> /home/hacker/the-flag` to redirect the output, then `cat /home/hacker/the-flag` to get the flag.

# Redirecting errors
Learnt about File Descriptor (FD)  which is a number the describes a communication channel in Linux \
Then used `/challenge/run > myflag 2> instructions` and `cat myflag`to get the flag.

# Redirecting input
Ran `echo COLLEGE > PWN` to redirect output to `PWN`, then from `PWN` redirected input to `/challenge/run` by `/challenge/run < PWN` to get the flag.

# Grepping stored results
Ran `/challenge/run > /tmp/data.txt` to redirect output to `/tmp/data.txt`, then  used `grep pwn /tmp/data.txt` to find the flag.

# Grepping live output
Learnt about pipe `|` operator \
`/challenge/run | grep pwn` to get the flag.

# Grepping errors
Ran `/challenge/run 2>& 1| grep pwn` to get the flag after redirecting standard error to output and then piping.

# Duplicating piped data with tee
This took a lot of time as I thought the value would pass directly into `/challenge/college` after a lot of tries,
I figured out that  after doing `/challenge/pwn | tee output | /challenge/college`, I  have to use `cat output`
which gives the output that `--secret` should be used with the secret arguement `ItzLP14X` \
On running `/challenge/pwn --secret ItzLP14X | /challenge/college`, I got the flag.

# Writing to multiple programs
Ran`/challenge/hack | tee >(/challenge/the) >(/challenge/planet)` to get the flag.

# Split-piping stderr and stdout
Ran `/challenge/hack 2> >(/challenge/the) > >(/challenge/planet)` to get the flag.
