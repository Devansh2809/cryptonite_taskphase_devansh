#Becoming Root with su
First ran `su` to switch user by entering the password `hack-the-planet` and on entering the root shell I used `cat / flag` to get the flag.

# Other Users with su
Ran `su zardus` and passowrd `dont-hack-me` to enter the user __zardus__ after which I entered `/challenge/run` to obtain the flag.  

# Cracking Passwords
Use `john /challenge/shadow-leak` to crack the password it reveals password to be `aardvark` switch user to zardus,enter the password then run `/challenge/run` to get the flag.

# Using sudo
Run`sudo cat /flag` to get the flag .

