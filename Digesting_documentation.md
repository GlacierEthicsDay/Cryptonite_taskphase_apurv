# Learning from documentation
A simple challenge that involved passing the argument --giveflag, this provided the flag.
# learning complex usage
In this challenge I simply replaced the end of the example statement- /challenge/challenge --printfile /challenge/DESCRIPTION.md with /flag to get the flag.
# Reading manuals
We use man command in this challenge to read manual of challenge and get clues on what to append after /challenge/challenge to get the flag, we have to write the specified string and 264 along with it to get the flag.
# Searching manuals
This challenges requires us to search through the manual of challenge to get the right argument, we use "/ flag" to find all places wherever flag is written and end up on the correct argument to get the flag.
# Searching for manuals
This challenge took me a few a attempts as I could not figure out how to search through man man, I used /challenge to see if I can use this to search but it didnt work so I read the initial few lines of man man by scrolling down to find clues, here -k caught my attention which is used as regex to find text after it, so I used it as man -k challenge to find the manual that has challenge word inside it, after getting the manual name we simply have to open it and find the correct argument for flag like the last challenges.
# helpful programs
This challenge involved using -h command to learn about programs without a man page, we simply use the -h command to find about /challenge where we find we first have to use the argument -p to get the integer value then use this with -g argument to finally get the flag.
# helpful for bulletins
This time /challenge is not a program rather a shell bulletin so we first use help challenge command to get info about it then rather doing /challenge/challenge --argument we simply do challenge --argument passing the correct secret phrase we got from help to get the flag.