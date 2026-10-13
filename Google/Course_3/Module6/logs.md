- The act of creating log events is called logging 

- The one log file that logs pretty much everything on your system is the /var/log/syslog file

- you can filter logs in order to see issues in a easier more efficient way for instance 'less /var/log/syslog | grep error' allows your to search for logs with the word error within them 

- use 'tail -f /var/log/syslog' to see logs in real time

- logs can be very useful when faced with a problem machine that leaves no obvious clues