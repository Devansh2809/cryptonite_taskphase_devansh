# Changing File Ownership
I first did `ls -l /flag` then I did `chown hacker /flag` to change its user to `hacker`, to get the flag I used `cat /flag`. 

# Groups and Files 
First did `ls -l /flag` after which I did `chgrp hacker /flag` to change its group to `hacker`, and then using `cat /flag` I got the flag. 

# Fun with Group Names
I first used `id` to get the information that  the group name is `grp13212` to chenge the group name I did `chgrp grp13212 /flag`  after which I used `cat /flag` to get the flag. 

# Changing Permissions
First used `ls -l /flag` to check the status of flag file, then used `chmod go+r /flag` to change the permissions, after which I ran `cat /flag` to get the flag. 

# Executable Files
First ran `ls -l /challenge/run` to check the permissions, then used `chmod a+x /challenge/run` to change the permissions to allow the file to be executable by all,after which I ran `/challenge/run` to to get the flag.

# Permission Tweaking Practise
I first ran `challenge/run` and then followed the steps as instructed, changing permissions accordingly when asked 
```
chmod o+w /challenge/pwn
chmod ug+wx /challenge/pwn
chmod o+x /challenge/pwn
chmod o-rw /challenge/pwn
chmod u-rwx /challenge/pwn
chmod u+rwx /challenge/pwn
chmod ug-w /challenge/pwn
chmod ugo-rwx /challenge/pwn
```
After all these steps I was asked to make the `/flag` file readable which  had no permissions so I did `chmod a+r /flag` and `cat /flag` to get the flag.

# Permission Setting Practise
I first ran `challenge/run` and then followed the steps as instructed, changing permissions accordingly when asked 
```
chmod o=rw,u=rx,g=w /challenge/pwn
chmod o=w,u=rwx,g=wx /challenge/pwn
chmod u=rx,g=wx,o=w /challenge/pwn
chmod u=rx,g=r,o=wx /challenge/pwn
chmod u=wx,g=r,o=x /challenge/pwn
chmod u=x,g=wx,o=x /challenge/pwn
chmod u=rwx,g=rx,o=r /challenge/pwn
chmod u=-,g=rwx,o=rx /challenge/pwn
```
After all these steps I was asked to make the `/flag` file readable which  had no permissions so I did `chmod a=r /flag` and `cat /flag` to get the flag.


# The SUID Bit
First I use `chmod ugo+s /challenge/getroot` to change SUID bit,after which I ran `/challenge/getroot` to set up the shell in which I used `cat /flag` to get the flag. 
