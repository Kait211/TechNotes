# Services
- DNS
- DHCP
- NTP
These run as background services also known as daemons or just services. This means that the programs doesn't need to interact with a user through the graphical interface or the command line interface to provide the necessary service.

Services are usually configured to start when the machine boots, so that if there's a power outage or a similar event that causes the machine to reboot, you won't need a system admin to manually start the service 

The configuration files for the installed services are located in the 
/etc directory

# lftp
An ftp client program that allows us to connect to an ftp server 

# reload 
The service re-reads the configuration without having to stop and start
That way ongoing connections aren't interrupted but ​new connections will use a new configuration

# Managing System Services in Linux

**Start:** Turns on a service so it can run. Example: Starting the SSH service.

**Stop:** Turns off a running service. Example: Stopping the SSH service.

**Restart:** Stops a service and starts it again. Useful when a service isn't working correctly or after changing settings.

**Reload:** Applies configuration changes without fully stopping and restarting the service. The service must support reloading.

**Modify Configuration:** Changes a service's settings by editing its configuration file. Changes may require a reload or restart to take effect.

### Example Commands

- `sudo systemctl start ssh` — Starts the SSH service.
- `sudo systemctl stop ssh` — Stops the SSH service.
- `sudo systemctl restart ssh` — Stops and starts the SSH service again.
- `sudo systemctl reload ssh` — Reloads the SSH service's configuration without fully restarting it.
- `sudo nano /etc/ssh/sshd_config` — Opens the SSH server configuration file for editing.
- `sudo systemctl enable ssh` — Configures SSH to start automatically when Ubuntu boots.

**systemctl:** A Linux command used to manage system services.

**sudo:** Runs a command with administrator privileges.

**Important:** Not all services support `reload`. If a service doesn't support it, you may need to use `restart` instead.

### dnsmasq
A program that provides DNS, DHCP, TFTP and PXE services in a simple package

# dnsmasq reference guide link
https://docs.google.com/document/d/1IlMrKgWltH37bYCJGCWJIZZwT7Y05fsuxsHL7tq_CJ4/edit?usp=sharing&resourcekey=0-hHy8_8D70uuhcIBOtVs2ew

