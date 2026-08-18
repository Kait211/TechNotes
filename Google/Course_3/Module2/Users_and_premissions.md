# Users and groups
### There are two different types of users
- standard users
- Administrators 

### Standard user
One who is given access to a machine but has restricted access to do things like install software or change certain settings

### Admin
A user that has complete control over a machine 

### Computer management 
allows you to make who is admin and who is standard user

![Computer Management Diagram](../../images/Computer_management.png)

### Windows domain
A network of computers, users, files, ect that are added to a central database 

### User Account Control (UAC)
A feature in Windows that prevent unauthorized changes to a system 

use CLI command Get-LocalUser to get info on all users and what their role is and permissions
and Get-LocalGroup will get groups on the machine

example for both
Get-LocalGroupMember Administrators

### Root User
First user that gets automatically created when we install a Linux OS

### sudo command or superuser do
allows a user to make commands like a root user
- if you use sudo -su, you can log in as root user

When you set a password it's securely scrambled, then stored in a special privileged file called /etc/shadow

# Permissions
In Windows, files and directory permissions are assigned using Access Control Lists or ACLs. Specifically, we're gonna work with Discretionary Access Control Lists or DACLs

Windows files and folders can also have System Access Control Lists or SACLs assigned to them

### Read
Lets you see that a file exists, and allows you to read it's contents. it also lets you read the files and directories 

### Read and execute
Lets you read files, and if the file is an executable you can run this file

Read and execute includes Read, so if you select Read and execute, Read will be automatically selected 

### List folder contents
An alias for Read and execute on a directory 

### Write 
Lets you make changes to a file

The Write permission also lets you create subdirectories, and write to files in the directory

### Modify 
The modify permission is an umbrella permission that includes read, execute, and write

### Full control 
A user or group with full control can do anything they want to the file

### Simple permissions
Sets of special, or specific permissions 
- WD: Create Files/Write data
- AD: Create Folders/Append Data
- S: Synchronize 