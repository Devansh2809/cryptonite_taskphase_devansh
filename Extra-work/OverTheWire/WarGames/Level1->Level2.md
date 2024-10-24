First use ls to see that `-` is the file to be catted but it cant be catted normally it has to be catted by `cat ./-` which gives us the password `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`. \ 
On getting the password I use `logout` to logout after which I establish a connection using `ssh bandit2@bandit.labs.overthewire.org -p 2220` and then put the password to login.
