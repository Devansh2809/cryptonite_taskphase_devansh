# Learning From Documentation
Ran `/challenge/challenge --giveflag` to get the flag.

# Learning Complex Usage
Learnt that arguements can have arguements of their own. \
Ran `/challenge/challenge --printfile /flag` to get the flag.

# Reading Manuals
Use `man challenge`. \ 
It states that I should use the arguement `tknpuy` and give it 194 to print the flag. \
Running the command `/challenge/challenge --tknpuy 194` gives the flag.

# Searching Manuals
Use `man challenge`.Search for `flag` in the manual using /,  which states  `--ph` will give the flag.

# Searching for Manuals
After running `man man`, I used all commands suggested in the synopsis to  understand that `-k` is the best option. Doing `man -k challenge` gives `osrcqsxsyt (1)`. \
Now using `man osrcqsxsyt` provides the information that using `--osrcqs` with 818 as arguement will give flag. Run `/challenge/challenge --osrcqs 818`

# Helpful Programs
Doing  `/challenge/challenge --help`. It gives some optional arguements in which is arguement `-p` which will give the value to use in `-g` to print the flag \
So after running `/challenge/challenge --p`, it prints
```
The secret value is: 878
```
On running  `/challenge/challenge -g 878` we get the flag.

# Help for Builtins
Running `help challenge`, gives the help page of this builtin. It instructs us to use the arguement `--secret` with its  value `w3IxhzH3` \
Running `challenge --secret w3IxhzH3` gives the value of the flag.
