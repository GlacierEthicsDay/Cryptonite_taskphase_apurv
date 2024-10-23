# changing file ownership
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{Y1CZ_Y6XIDt5gD6J0-Vm5SmnChY.dFTM2QDLwgDO0czW}
# groups and files
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{sf7NmdZPKgoZvFCDo-1o1ze8_6X.dFzNyUDLwgDO0czW}
# fun with group names
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp30650) groups=1000(grp30650)
hacker@permissions~fun-with-groups-names:~$ chgrp grp30650 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{8ltoJzGvrLdlJbwzz44p2xXI_tw.dJzNyUDLwgDO0czW}
# changing permissions
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{s2B2ng_7aaFm5gVy23l2YFXFKdK.dNzNyUDLwgDO0czW}
# executable files
hacker@permissions~executable-files:~$ chmod o+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
bash: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{A4ulRZ0gTam-GVm30HknE84Oa8-.dJTM2QDLwgDO0czW}
# tweaking permissions
This was a very a long challenge that involved changing file permissions over 8 times to finally get the desired permissions and then finally changing permission of flag file to make it readable to get the flag.
pwn.college{0tdwffOkP2AL6JFoNXlYOSMwV8Z.dBTM2QDLwgDO0czW}
# suid
For this challenge we use chmod to add suid for root user using chmod like this-
chmod u+s /challenge/getroot
then we-
/challenge/getroot
and then cat the flag to get the flag.
pwn.college{oMoGkBQP9be-M3BDMxYngSTom-7.dNTM2QDLwgDO0czW}
