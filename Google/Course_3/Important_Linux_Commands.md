# Linux Commands for IT Help Desk

## 📁 Navigation & Files

**`pwd`**: Shows your current directory

```bash
pwd
```

**`ls`**: Lists files and folders

```bash
ls
ls -la
```

**`cd`**: Changes to another directory

```bash
cd Documents
cd ..
cd ~
```

**`mkdir`**: Creates a new directory

```bash
mkdir new_folder
```

**`touch`**: Creates a new empty file

```bash
touch test.txt
```

**`cp`**: Copies files or folders

```bash
cp file.txt backup.txt
cp -r folder1 folder2
```

**`mv`**: Moves or renames files

```bash
mv old.txt new.txt
```

**`rm`**: Deletes files

```bash
rm file.txt
rm -r folder
```

**`find`**: Searches for files and directories

```bash
find /home -name "test.txt"
```

---

## 📄 Viewing & Editing Files

**`cat`**: Displays the contents of a file

```bash
cat file.txt
```

**`less`**: Views a file one screen at a time

```bash
less file.txt
```

**`head`**: Shows the beginning of a file

```bash
head file.txt
```

**`tail`**: Shows the end of a file

```bash
tail file.txt
```

**`nano`**: Simple terminal text editor

```bash
nano file.txt
```

---

## 🔐 Permissions & Users

**`chmod`**: Changes file permissions

```bash
chmod u+w file.txt
```

**`chown`**: Changes file owner

```bash
sudo chown user file.txt
```

**`whoami`**: Shows the current user

```bash
whoami
```

**`id`**: Shows a user's ID and group information

```bash
id
```

**`sudo`**: Runs a command with administrator privileges

```bash
sudo command
```

**`passwd`**: Changes a user's password

```bash
passwd
```

---

## ⚙️ Processes

**`ps`**: Shows running processes

```bash
ps
ps aux
```

**`top`**: Shows processes and system resource usage in real time

```bash
top
```

**`kill`**: Sends a signal to a process

```bash
kill 342
```

**`kill -9`**: Forcefully terminates a process

```bash
kill -9 342
```

**`jobs`**: Shows processes running in the current shell

```bash
jobs
```

**`fg`**: Brings a background process to the foreground

```bash
fg
```

---

## 🌐 Networking

**`ip`**: Shows or manages network information

```bash
ip addr
ip route
```

**`ping`**: Tests whether another device can be reached

```bash
ping google.com
```

**`traceroute`**: Shows the path packets take to another device

```bash
traceroute google.com
```

**`ss`**: Shows network connections and listening ports

```bash
ss -tuln
```

**`curl`**: Connects to a URL and transfers data

```bash
curl https://example.com
```

**`dig`**: Looks up DNS information

```bash
dig google.com
```

**`nslookup`**: Looks up DNS information

```bash
nslookup google.com
```

---

## 💾 Disk & Storage

**`df`**: Shows available disk space

```bash
df -h
```

**`du`**: Shows how much space files/directories use

```bash
du -sh folder
```

**`lsblk`**: Lists disks and partitions

```bash
lsblk
```

**`mount`**: Mounts a filesystem

```bash
mount
```

**`umount`**: Unmounts a filesystem

```bash
sudo umount /dev/sdb1
```

**`free`**: Shows RAM and swap usage

```bash
free -h
```

---

## 📦 Software & Updates

### Debian/Ubuntu

**`apt update`**: Updates the package list

```bash
sudo apt update
```

**`apt upgrade`**: Installs available package updates

```bash
sudo apt upgrade
```

**`apt install`**: Installs a package

```bash
sudo apt install package-name
```

**`apt remove`**: Removes a package

```bash
sudo apt remove package-name
```

---

## 📝 Logs & Troubleshooting

**`journalctl`**: Views system logs

```bash
journalctl
```

**`dmesg`**: Shows messages from the Linux kernel

```bash
dmesg
```

**`history`**: Shows previously entered commands

```bash
history
```

**`grep`**: Searches for text inside output or files

```bash
grep "error" logfile.txt
```

**`which`**: Shows where a command is located

```bash
which python
```

---

## 🔎 System Information

**`uname`**: Shows information about the Linux system

```bash
uname -a
```

**`hostname`**: Shows the computer's hostname

```bash
hostname
```

**`uptime`**: Shows how long the system has been running

```bash
uptime
```

**`date`**: Shows the current date and time

```bash
date
```

**`lscpu`**: Shows CPU information

```bash
lscpu
```

---

## 🔧 Useful Help Commands

**`man`**: Opens the manual for a command

```bash
man ls
```

**`command --help`**: Shows basic help for a command

```bash
ls --help
```

**`clear`**: Clears the terminal screen

```bash
clear
```

---

## 🔗 Pipes & Redirection

**`|` (Pipe)**: Sends the output of one command into another command

```bash
ls | grep ".txt"
```

**`>`**: Sends output into a file and overwrites it

```bash
ls > files.txt
```

**`>>`**: Adds output to the end of a file

```bash
ls >> files.txt
```

**`<`**: Uses a file as input

```bash
command < file.txt
```

---

## ⭐ Commands to Know First

If you're preparing for an **IT help desk job**, focus on these first:

```text
pwd
ls
cd
cp
mv
rm
mkdir
cat
less
grep
find
chmod
chown
sudo
whoami
id
ps
top
kill
ip
ping
traceroute
ss
df
du
lsblk
free
apt
journalctl
uname
history
man
```

**Help desk mindset:** A lot of Linux troubleshooting comes down to checking **files, permissions, users, processes, networking, disk space, and logs**.
