# Redirecting output
This challenge introduced the ">" command which used to print the output to a file, for this challenge we had to output "PWN" on the file "College" to get the flag.
# Redirecting more output 
This challenge was similar to last one, we had to print output of /challenge/run on the file /myflag then simply use cat command to read this file for the flag.
# Appending output
This challenge introduced the ">>" command which is used to append output to the the same file, we simply had to use this for /challenge/run then use cat command to read the-flag file for the flag.
# Redirecting error
This challenge involved directing out and error of the the /challenge/run to 2 different files using the command /challenge/run >> /home/hacker/the-flag, after this we use cat command to read the flaq file to get the flag.
# Redirecting Input
This challenge involved first writing COLLEGE into the PWN file then using < to redirect this to /challenge/run file to get the output.
# Grepping stored Results
This challenge involved redirecting output of /challenge/run to a text file then using grep command to find the flag, this is achieved by using grep pwn (filename).
# Grepping live results
This challenge introduced the piped operator, we simply do /challenge/run | grep pwn to run and grep the flag.
# grepping errors
This challenge involved redirecting output of standrard error to standard output then simply grepping for the flag.
# duplicating piped data with tee
This challenge teaches us about command tee, using the command we are told we need to have a sceret code to successfully get the flag, we get get this flag from output1 file, the final command being /challenge/pwn --secret c8rZcshb | /challenge/college to get the flag.
# writing to multiple programs 
THis challenge involved redirecting output of /challenge/hack into to files at once using tee substitution, we achieve it by using the /challenge/hack | tee >( /challenge/the ) >( /challenge/planet ) command to get the flag.
# Split piping
This was a tricky challenge that involved redirecting output of error and output of challenge hack into challenge/the and challenge/ planet, this was achieved by using the command /challenge/hack 2> >( /challenge/the ) 1> >( /challenge/planet ), we need to use process substitution to get the flag.
