# The Root
Invoke the pwn program using its absolute path by using  `pwn`

# Program and absolute paths
Invoke the `run` program to execute the run file that is in the challenge directory that is, in turn, in the / directory by entering its path, `/challenge/run`.

# Position thy self
Learned to navigate around directories by using the cd (change directory) command \
Using the `/challenge/run` gives an error as follows
```
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
```
After using `cd /usr/share/doc` to naviagte to the directory,  run `/challenge/run`.

# Position elsewhere
Running the `run` program as before,outputs that we are running the `run` program from a different directory \
Using the `/challenge/run` gives an error as follows 
```
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
```
After using `cd /tmp` to naviagte to the directory,  run `/challenge/run`.


# Position yet elsewhere
Running the `run` program as before,outputs that we are running the `run` program from a different directory \
Using the `/challenge/run` gives an error as follows 
```
Incorrect...
You are not currently in the /etc directory.
Please use the `cd` utility to change directory appropriately.
```
After using `cd /etc` to naviagte to the directory,  run `/challenge/run`.

# Implicit relative paths, from /
Learned that the current working directory does matter for relative paths \
After navigating to `cd /` run the command `/challenge/run`

# Explicit relative paths, from /
`.` refers to the same directory \
Use the command `./challenge/run` to get the flag.

# Implicit relative path
After navigating to `cd /` I thought I would try `./challenge/run` which resulted in an error stating I am not correctly in challenge directory \
On understanding this I used `cd challenge` to go into challenge and then used `./run` to run the file using relative path

# Home sweet home
After navigating to `cd /` ,not completely understanding the question correctly I first ran `/challenge/run` which gave an error that some arguement must be specified, on understanding the error i understood that I would have to use `/challenge/run ~/d` where d is an arguement provided to which the file is written and `~` is the absolute path of home directory
