# Matching with *
First run `cd /ch*` which took me into `challenge` directory. Then run `/challenge/run` to get the flag.

# Matching with ?
Running `cd /?ha??enge`took me to the `challenge` directory, then `/challenge/run` gives the flag

# Matching with []
First change  to `/challenge/file` directory, then use `/challenge/run file_[bash]` to get the flag.

# Matching paths with []
Run`/challenge/run /challenge/files/file_[bash]` to get the flag .

# Mixing globs
Go into `/challenge/files`. \
Using `/challenge/run *[i]*` gives many more words which are not required like 
```
amazing beautiful challenging delightful educational fantastic incredible jovial kind laughing magical nice optimistic pwning radiant splendid thrilling uplifting victorious xenial
```
Then I used `/challenge/run [cep]*` to get the flag.

# Exclusionary globbing
Go into `/challenge/files`, then run `/challenge/run [^pwn]*` to get the flag.
