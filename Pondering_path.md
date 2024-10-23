# the path variable
For this challenge we need to clear the path variable then run the challenge run file like this-
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{kBGjb9u3Akc7AHUaw78w1h3vdB1.dZzNwUDLwgDO0czW}
# setting path
Instead of keeping path variable empty, we assign a value to it and then run challenge run file.
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{ocpATUMYx9P9-jCQSJ1ddnE6hDD.dVzNyUDLwgDO0czW}
# adding commands
Like previous module, we create bash script to display output of cat\flag then we use chmod to make it a executable file, we finally update the path variable and run the challenge run file to get the flag.
pwn.college{8IM0afEEBX9tcQlTkuxv13wGBh3.dZzNyUDLwgDO0czW}
# Hijacking commands
To solve this challenge we need to create a pseudo rm command that prevents the original from deleting. We also need to update the path variable to prioritise our pseudo rm instead of orginial by adding our value before $PATH while defining path.
pwn.college{4HKNgCgNOFsSskOUNpAQCQu30Sq.ddzNyUDLwgDO0czW}
