# Listing Processes
Ran `ps -ef` to get the list of all processes, out of all of them I ran `/challenge/15339-run-27510` to get the flag.

# Killing Processes
Use `ps -aux` to get the list of the processes then using the __PID__ of the process kill it `kill 73` and run `/challenge/run` to get the flag.

# Interrupting Processes
First run `/challenge/run` which says it willl give me the flag on interrupting the process so I use `ctrl+c` to interrupt and am provided with the flag. 

# Suspending Processes
Running `/challenge/run` will give 
```
I'll only give you the flag if there's already another copy of me running in
this terminal
```
Asks me to `ctrl+z` after which i again run `/challenge/run` on doing so I get the flag.

# Resuming Processes
On running `/challenge/run` it tells me to first interrupt the process after which I use `fg` to resume it back to get the flag.

# Backgrounding Processes 
Ran `/challenge/run` it told me to first interrupt the process then run it in background which i did by `bg /challenge/run` and then I used `/challenge/run`  to get the flag.

# Foreground Processes 
Ran `/challenge/run` then interrupted the process and then ran it in the  background by `bg /challenge/run` after that it asked me to run it in the foreground using `fg /challenge/run` and then I pressed enter to get the flag.

# Backgrounding Processes 
Ran `/challenge/run` it told me to first interrupt the process the run it in background which i did by `bg /challenge/run` and then I used `/challenge/run`  to get the flag.

# Starting Backgrounded Processes 
Did `/challenge/run &` to to start the backgrounded process and get the flag.
