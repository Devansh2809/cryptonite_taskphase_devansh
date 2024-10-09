# Printing Variables
Ran `echo $FLAG` to get the flag.

# Setting Variables
Ran `PWN=COLLEGE` to get the flag.

# Multi-word Variables
Ran `PWN="COLLEGE YEAH"` to get the flag.

# Exporting Variables
Ran the commands
```
COLLEGE=PWN
PWN=COLLEGE
export PWN
sh
/challenge/run PWN
```
to get the flag

# Printing Exported Variables
Ran `env` to find the flag in the list of variables.

# Storing Command Output
Ran `PWN=$(/challenge/run)` to store the output of the command in the variable, then `echo "$PWN"` to get the flag.

# Reading Input
Ran `read PWN` to accept input, then inputted `COLLEGE` to get the flag.

# Reading Files
Ran `read PWN < /challenge/read_me` to redirect the file to the `PWN` variable as input and gives the flag.
