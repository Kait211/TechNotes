# Operating System
The Whole package that manages our computer's resources and lets us interact with it 

### There are two main parts to an operating system
- The Kernal: ​The kernel is the main core of an operating system. ​It talks directly to our hardware and manages our system's resources
- The user space: The user space is basically made up of everything outside the kernel. ​These are things that we interact with directly like system programs, ​user interfaces, etcetera. ​

### The main operating systems are
- Windows 
- Mac
- Linux (open source): some common Linux distributions are Ubuntu, Debian, and red hat

### The Kernel
- The kernel handles storing and organizing files on a computer.

- A file is just data, like a document, picture, or song.

- A file system is how those files are organized so they aren’t all mixed together—like using folders in an office instead of dumping everything into one cabinet.

- Another important function of the kernel is process management. ​We have many programs that we want to run on our system. ​To run them we manage the order they run in, how many resources they take up, ​how long they run etcetera. ex typing while listening to music

- Our Kernel optimizes Memory usage and makes sure our applications have enough memory to run

- The last important function that a kernel performs is input, output or IO management ​

- IO Management: Anything that can give us input, or that we can use for output of data 

Summary:
The Kernel is reponsible for
- File management 
- Process management 
- Memory management 
- I/O management 

### There are three main components to handling files handlers
- The file data 
- Metadata
- File system

- major OS manufacturers have ​their own unique file systems that they recommend, ​for Windows, the major file system that's used is NTFS. ​It was introduced in the previous version of Windows OS, ​Windows NT, and includes many features like encryption, ​faster access speeds, security, and more

- We write data to our hard drive in the form of data blocks 

### Block storage
Improves faster handling of data because the data isn't stored as one long piece and can be accessed quicker 

- ​Lastly, we need to keep the metadata ​that contains the information about our file. ​There's a lot of information ​about our file that we want to know, ​who created it, when it was last modified, ​who has access to it, and so on. ​The file metadata tells us ​everything we need to know about our file. ​It also tells us what type of file it is.

### File extension 
The appended part of a filename that tells us what type of file it is in certain operating systems 

### Program
An application that we can run like Chrome

### Process
A program that's executing, like our internet browser or text editor 

- ​This process needs to have ​hardware resources like RAM and CPU. ​The kernel has to schedule time for the CPU to ​execute the instructions in the process, ​but there's only one CPU and many processes. ​How is the CPU able to execute ​multiple processes at once? It actually doesn't. ​It executes processes one-by-one ​through something known as a time slice.
 ### time slice
  is a very short interval of time that ​gets allocated to a process for CPU execution. ​It's so short that you don't even notice it. 

  ### Kernel
  Creates processes, efficiently schedules them and manages how processes are terminated 

  ### Virtual memory
  The combination if hard drive space and RAM that acts like memory that our processes can use 

  - When we execute a process, ​we take the data of the program in chunks we call **pages**. ​We store these pages in virtual memory. 

  - The Kernel handles the process of taking pages of data and swapping them between RAM and ​virtual memory. 

### I/O devices
Devices that perform input and output
-  ​When the kernel is able to start the drivers to communicate with hardware, ​it also manages the transfer of data in and out of the devices
- Our kernel handles all the inter communication between devices. ​It also figures out what the most efficient method of transfer is and ​it tries its best to make sure our data doesn't have errors during process.

- When you're troubleshooting or solving a problem with a **slow machine**, it's usually some sort of **hardware resource deficiency**

- if you don't have enough RAM you can't load up as many processes. ​If you don't have enough CPU you can't execute programs fast enough. ​If you have too much input coming into the device or too much output going somewhere ​you'll also block other data from being sent or received. Beyond desktop support, identifying the source of a resource bottleneck and ​a server or large IT system like a Web application can unlock performance gains ​and new heights of responsiveness for your users. 

### There are two ways that we can interact with our OS
- Shell (CLI: Command line interface)
- Graphical user interface: a visual way to interact with the computer. 

### Shell
A program that interprets text commands and sends them to the OS to execute, the most common shell is Bash or bourne 

### Logs
Files that record system events on our computer, just like a system's diary 
- A computer will record events like when it was turned on, when a driver was loaded. ​And even when something isn't working in the form of error messages. ​

-  ​As an IT support specialist, ​you'll probably work on lots ​of computers that won't start, booting is when your start up the computer

### ​Here's a rundown of the boot process. 
​First, the computer is powered on. ​The BIOS/UEFI is a low-level software that ​initializes our computer's hardware ​to make sure everything is good to go. ​Next, the bios UEFI runs a process called the ​power-on self-test, or post. ​The post performs a series of diagnostic tests to ​make sure that the computer is in proper working order. ​Next, depending on the bios or ​UEFI configuration of boot device will be selected. 
​Devices that are attached to ​our system, like hard drives, ​USB drives, CD drives, ​etc, are configured in a certain boot order. ​The devices will be checked in this order and ​the computer will search for ​what's known as a bootloader. ​The bootloader is a small program ​that loads the operating system. ​Once our computer finds ​a bootloader on a device in the listed order, ​it will start to execute this program. ​This will then start to load ​a larger and more complex program ​and eventually loads our operating system. ​Once the bootloader loads up our operating system, ​our kernel gets loaded. ​The kernel controls access to our computer's resources. 
​It also loads up drivers and more so ​that our hardware can talk to our software. ​Next, essential system ​processes and user space items are launched. ​These include processes like user login, ​spinning up a desktop environment, ​and more which basically ​allows us to interact with our system. ​And that's it. After these simple steps, ​you'll be able to get to work. 

### BIOS/UEFI
A low-level software that initializes our computer's hardware to make sure everything is good to go 

### Bootloader
A small program that loads the operating system

- Boot order is the order in which a computer chooses which boot files to use to startup. The boot order determines your boot method. To set the boot order for a computer, you need to enter the BIOS and configure the boot options.

- o enter your computer’s BIOS on a Windows or Linux computer, power on the system and look for an on-screen message that says which function key you should press to enter setup. The function keys used for entering the BIOS vary between computer manufacturers and the version of BIOS. Some of the more common function key messages are "Press DEL to enter SETUP," "F2=SETUP," or "Press F12 to enter SETUP." If booting macOS, press and hold the Option key at startup. This will open up the Startup Manager, which will scan your computer and identify bootable devices. Then you can choose the bootable device you want to use.

- The BIOS screen will vary depending on your computer manufacturer and BIOS version, but all BIOS programs will feature a Boot Options menu. The Boot Options menu is where you can set your preferred boot method.The boot options menu lists all the devices attached to your system where it may find a bootloader program. These include devices like internal hard drives, USB drives, CD drives, as well as other storage options, like network storage or cloud storage. 

# You may find the following boot methods listed in your BIOS boot options: 
### External options 
- **USB drive**: You use a USB drive loaded with resources needed to boot the computer. This drive is inserted into a USB port and chosen at startup.
- **Optical Media**: You use an optical media disk loaded with booting resources. This disk can be a DVD, CD, or Blu-ray disk and is loaded through the computer's optical drive.

- **Solid State Boot Drive**: You can use a solid state drive to boot your computer. Solid state drives do not use spinning discs or moving parts. This solid state drive can be installed in the computer or can be a smaller device such as a flash drive.

- **External hot-swappable drive**: You may boot from an external hard drive that can be moved between computers without turning it off.

- **Network boot**: You can boot an operating system directly from a local area network (LAN) without using a storage device. Your computer must be connected to a LAN for this option. The network boot is used when the computer does not have an OS installed, among other things. To boot from a network, you will need to set up the Preboot Execution Environment (PXE) capability on the BIOS and have the network environment prepared for this type of request (see resources linked below).

- **Internet-based boot**: You boot the computer from an internet source, as long as it is a secure source. If you are in charge of a network and your server is down for any reason, you can use this boot method to remotely power on the server and restart network operations. Internet-based boot can be achieved in one of two ways:

- **Disk partitions**: You can create partitions on your computer’s drive so that only one part of the drive runs the boot process. A common reason to partition your drive is to have two separate operating systems on your computer. For example, you could have Windows on one partition of your drive and Linux on the other. When you have two operating systems on your drive, you must choose which one will run the boot process. Having two possible systems to boot into is called dual booting.