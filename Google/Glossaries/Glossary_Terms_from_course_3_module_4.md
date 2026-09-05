# Storage and File Systems Glossary

* **Command line mode:** When you are able to run commands while still in your current shell.

* **Data:** The actual content of a file.

* **Data buffer:** A region of RAM used to temporarily store data while it is being moved around.

* **Defragmentation:** A process of reorganizing files on a disk so their data is stored in neighboring locations.

* **Disk Management utility:** A native Windows tool used to manage disk space, partitions, and volumes.

* **File record number:** The index of a file's entry in the MFT.

* **File system:** Used to keep track of files and how they are stored on a disk.

* **Hard link:** In NTFS, an entry added to the MFT that points to the linked file's record number rather than its name. This means the target file can be renamed and the hard link will still point to it.

* **Inode:** A file structure that stores metadata about a file and information about its data.

* **Interactive mode:** When the `parted` tool launches you into a separate program where you can enter commands.

* **Master Boot Record (MBR):** A traditional partition table stored on a disk. It supports volume sizes of up to about 2 TB and is commonly associated with older Windows systems.

* **Master File Table (MFT):** A structure used by NTFS to store information about the files on a disk.

* **Memory manager:** A Windows OS component that helps manage virtual memory.

* **Metadata:** Information about a file, such as who created it, when it was last modified, who has access to it, and what type of file it is.

* **Mounting:** Making a file system or storage device accessible to the computer.

* **Partition table:** Information that describes how a disk is divided into partitions.

* **Shortcut:** A Windows entry that contains a reference to a destination, allowing you to open the shortcut and be taken to that destination.

* **Soft link:** A Linux shortcut that allows you to link to another file using its filename.

* **Swap space:** Allocated storage space used for virtual memory when physical RAM is full or heavily used.

* **Symbolic link:** A link that works similarly to a shortcut but operates at the file-system level. The operating system generally treats it as a substitute/reference for the file it points to.

* **System properties:** A Windows control panel area that allows you to edit the size, number, and location of paging files.

* **TRIM:** A command that tells a storage device which data blocks are no longer being used so they can be reclaimed.

* **UEFI:** A modern replacement for the traditional BIOS firmware interface.

* **UUID:** Universally Unique Identifier; a unique identifier used to identify things such as storage partitions.

* **Virtual memory:** A combination of RAM and storage space that the operating system can use as memory for processes.

* **Volume:** A storage area formatted with a file system that the operating system can use to store files.
