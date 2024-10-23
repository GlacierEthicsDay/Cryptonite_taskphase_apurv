# chaining with semi colon
This challenge teaches you can use semicolon to chain commands, we use " /challenge/pwn; /challenge/college" to get the flag.
pwn.college{M0LmhfNFQi_J-1v-lp1B_LgfT0t.dVTN4QDLwgDO0czW}
# first shell script
This challenge requires to open a text editor and use the command in previous challenge to be saved inside a file called x.sh then run the bash file for the flag.
pwn.college{kUE0vMyGPS6niJYmrUZ2lKhJIB5.dFzN4QDLwgDO0czW}
# Redirecting script output
Same as last challenge but we pipe the solve along with our bash script.
 bash x.sh | /challenge/solve
pwn.college{oYTy2egqSaOu5EV0zBJCXhutRgL.dhTM5QDLwgDO0czW}
# executable shell scripts
Again we create a .sh file but this time we use chmod to give it execute permissions to get the flag.
hacker@chaining~executable-shell-scripts:~$ chmod +x solve_script.sh
hacker@chaining~executable-shell-scripts:~$ ./solve_script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{sMusfphW8JTyQt1dNz9a3hGrmeq.dRzNyUDLwgDO0czW}
