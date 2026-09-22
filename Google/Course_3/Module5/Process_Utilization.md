# uptime
Linux uses three decimal values to show the load over time instead of the percent other systems use. An easy way to check the load average is to run the uptime command in the terminal. The following image depicts the load values returned from the uptime command. 

The command returns three load averages:

1. Average CPU load for last minute, which corresponds to 0.03. This is a very low value and means an average of 3% of the CPU was used over the last minute. 

2. Average CPU load for last 5 minutes corresponds to the second value of 0.03. Again, this can be thought of as, on average, 3% of the CPU was being used over the past five minutes. 

3. Average CPU load for last 15 minutes corresponds to 0.01, meaning on average, 1% of the CPU has been used over the last 15 minutes. 

# top
Another way you can monitor the load average in Linux is to use the top (table of processes) command in the terminal. The result of running the top command is an in-depth view of the resources being used on your system. 

The first line displayed is the same as the load average output given using the uptime command It lists what percent of the CPU is running processes or has processes waiting. The second line shows the task output and describes the status of processes in the system. The five states in the task output represent:

1. Total shows the sum of the processes from any state. 

2. Running shows the number of processes currently handling requests, executing normally, and having CPU access.

3. Sleeping shows the number of processes awaiting resources in their normal state. 

4. Stopped shows the number of processes ending and releasing resources. The stopped processes send a termination message to the parent process. The process created by the kernel in Linux is known as the “Parent Process.” All the processes derived from the parent process are termed as “Child Processes.”

5. Zombie shows the number of processes waiting for its parent process to release resources. Zombie processes usually mean an application or service didn't exit gracefully. Having a few zombie processes is not a problem. 

The top command gives detailed insight on usage for an IT individual to gauge the availability of resources on a system. 

