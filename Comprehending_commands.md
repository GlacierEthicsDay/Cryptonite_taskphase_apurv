# cat
This challenge simply gives an introduction to cat command, using it to read the flag file.
# catting absolute paths
Same as last challenge but this time we use the cat command on a absolute path to the flag file.
# catting more practice
In this challenge the path to flag file isnt given in the question but when running the vscode terminal the path is provided to us, we simply use cat command with the path to get the flag.
# grepping for a needle in a haystack
This challenge teaches to use grep command to search through big text files, clear hint is provided that flags start with pwn.college so we simply use grep command to search for this in the data.txt file.
# listing files
This challenge introduces the la command, we simply use it list out files present in challenge folder then open the rename run file.
# touching files
This challenges introduces the touch command, we simply create 2 folders inside tmp directory using it then go back the home directory and run the flag file.
# removing files
THis challenge introduces the rm command, we use it to delete the mentioned file  then run the "check" file to get the flag.
# hidden files
This challenge introduces ls -a command to list out hidden files, we use it find the flag file inside / directory and then we are required to use the cat command to read it since we don't have the permission to run the file.
# epic file quest game
This challenge was the longest challenge so far, it required to ls -a into a number of directories then use cat command to read the clue file, each clue file gave another clue, some clues had to be read by first using cd command to enter into the directory while some clues mentioned explicitly to not CD into the directory rather just use ls -a command to list out the file then use cat and its path to read it. Following this sequence we finally find the flag.
# making directories
This challenge introduced mkdir command which is used to make a directory, we make a directory inside /tmp then create a file using touch command inside it, when we complete this we run the /challenge/run to find the flag
# Finding files
This challenge was a slightly long challenge which required us to use the find command, to find the flag I first did "find / -name flag" this listed alot of directories ending in flag, I started to cd into each hoping to the flag until one responded back as "this is not a directory", I simply use cat command on this file and found the flag.
# linking files
In this challenge we learn to use ln -s command to link files. the /catflag is linked to /not-the-flag so here I used the ln -s command to link not-the-flag to /flag so when /catflag is used we end up reading from /flag as intended as its given the flag is inside /flag.
