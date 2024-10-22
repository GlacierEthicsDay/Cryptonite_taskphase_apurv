# listing processes
In this challenge, ps -ef command was used to find the renamed challenge run file, then we just run the renamed file.
pwn.college{UixigYtBdYxxKXEv20D13R_mqGm.dhzM4QDLwgDO0czW}
# killing processes
In this challenge, we first find the dont_run process by using the command  ps -ef | grep /challenge/dont_run, after which we gets its id and use kill command to kill it and run challenge file to the flag.
# interrupting processes
This challenge involved simple use of ctrl+c command to interrupt the process and get the flag.
pwn.college{AtgZNd4Ka09zKiyX7gYSFZWlh9G.dNDN4QDLwgDO0czW}
# suspending processes
This challenge uses ctrl+z to suspend a process, running another instance of run file while one is suspended gives the flag.
pwn.college{sOS4upx7OrScEnGZJTfvaxLITyG.dVDN4QDLwgDO0czW}
# Resuming processes
This challenge introduces the "fg" command to resume a suspended process, this gives the flag.
pwn.college{gNtgxf6aDfNjA13odWQTpn7CrTb.dZDN4QDLwgDO0czW}
# backgrounding processes
This challenge uses the "bg" command, we start the run process then suspend by ctrl+z and then send it to background then we start another run process to get the flag.
pwn.college{0fryJ26T3KV_fNzaq2mx8OT51ZI.ddDN4QDLwgDO0czW}
# foregrounding processes
This challenge introduces the "fg" command, we do the same steps as last time but instead of starting another process we use "fg" command to get the flag.
pwn.college{ksqljyPpOMNq9-y1C9GeEbYmNa5.dhDN4QDLwgDO0czW}
# starting backgrounded processes
This challenge introduces "&" command, we use this to start run as backgrounded process to get the flag.
pwn.college{0um62VIRBiXlIbJuqfeaaoSlZib.dlDN4QDLwgDO0czW}
# process exit codes
This challenge introduces $? command used to get process exit code, this used as argument to run another program to get the flag.
pwn.college{Qpbsi4zzBA095GF8k2Ph0wGw8Ij.dljN4UDLwgDO0czW}
