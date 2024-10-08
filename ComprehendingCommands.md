# Cat: not the pet, but the command!
Learned about `cat` which is used for reading out files and which will concatanate files if multiple arguements are given. \
Get the flag by running `cat flag`.

# Catting absolute paths
Get the flag by running `cat /flag`.

# More catting practice
Get the flag by running `cat /opt/libslub/libslub/flag`.

# Grepping for a needle in a haystack
`grep` command is used to search for content in big files. \
As all flags start with `pwn.college` Get the flag by running `grep pwn.college /challenge/data.txt`.

# Listing files
`ls` will list files in all the directories provided to it as arguments. \
List all files in `/challenge` using the command  `ls /challenge`, it gives two files, one of the files is named `17290-renamed-run-12529`. \
Get the flag by running `/challenge/17290-renamed-run-12529`.

# Touching files
Create  files using `touch /tmp/pwn` and `touch /tmp/college` then get the flag by running `/challenge/run`.

# Removing files
Use `rm delete_me` to remove the files, then get the flag by running `/challenge/check`.

# Hidden files
Go into `/` directory, run `ls -a`, the flag is hidden in file `.flag-88823059815822`. \
Use `cat .flag-88823059815822` to read the flag.

# An Epic Filesystem Quest
Move into `cd /` \
After using `ls -a`  many files are displayed but `NUGGET` files seems important so I use `cat NUGGET` which tells me to go the directory `/opt/kropr/.git/logs`  for the next clue   
I `cd /opt/kropr/.git/logs` to that directory, `ls -a` reveals a  hidden file named `.README` on using `cat .README`, the directory (`/usr/share/locale/ki/LC_MESSAGES`) contains the next clue \
After I do `cd /usr/share/locale/ki/LC_MESSAGES`,I used `ls -a` which had a file `GIST` after using `cat GIST`, a directory (`/usr/share/doc/libattr1`) was specified which had the next clue   
On going into the directory, I use `ls -a`and a file called  `TIP` seems like it contains the next directory, which it does (`/usr/local/lib/python3.8/dist-packages/sympy/interactive/tests`)  
After getting into the directory I use `ls -a` which gives a file `TRACE`, on using `cat TRACE` it shows a directory `/opt/linux/linux-5.4/drivers/net/ethernet/mellanox` \
After entering the directory I use `ls -a` which shows a hidden file `.MEMO`, on using `cat .MEMO` it shows a directory `/usr/local/lib/python3.8/dist-packages/capstone/include` .  \
On entering the directory, `ls -a` shows a file named `WHISPER`, on using `cat WHISPER` it shows a directory `/usr/share/man/fi/man1` .  \
Making my way into the directory, `ls -a` shows a file named `NOTE`, on using `cat NOTE` it shows a directory `/usr/share/racket/pkgs/games/blackjack` .  \
Use `ls /usr/share/racket/pkgs/games/blackjack` to get the files without using cd, which gives `ALERT-TRAPPED`, then `cat /usr/share/racket/pkgs/games/blackjack/ALERT-TRAPPED` gives me the flag. 

# Making directories
First I make a directory using `mkdir /tmp/pwn` \
Then I `cd` into this directory create a college folder by `touch college` \ 
Then I run `/challenge/run` to get the flag

# Finding files
Ran `find / -name flag` to find all files named flag in the system. \
It gave many possible directories some of them accesible most of them not I looked inside each usable directory by using `ls -a` \
The files inside had to be checked by using `cat` command most of them were not the required file but the file inside `/opt/linux/linux-5.4/include/linux/soc/dove/flag` contained the flag.

# Linking files
Learnt about the usage of  `links` via `hard and soft` links
On doing `ln -s /flag /home/hacker/not-the-flag` a symbolic link gets created, then running `/challenge/catflag`,  returns the flag.
