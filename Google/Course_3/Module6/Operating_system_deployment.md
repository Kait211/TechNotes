- One tool we can use to image computer is a disk cloning tool

-  ​It makes a copy of an entire disk and allows ​you to backup a current machine or set up a new one

- One of the many disk cloning tools out there ​is the open-source software clone Zillow. ​It can be used to backup and restore ​a single machine or many machines simultaneously. ​A popular commercial imaging tool is semantic ghost. 

-  you can use the Linux command line tool dd to copy files. ​Dd is a lightweight tool ​that's also used to clone a drive.

- ​If you're managing the operating ​system deployment for a company, ​you'll want to keep some aspects of ​hardware standardization in mind.

- ​When a mobile devices is built, ​it's installed with an operating system at the factory. ​So a factory reset returns the device back to the state it was in when the device ​well shipped from the factory, you'll have to factory reset mobile devices a lot. ​As an IT Support Specialist, you might do this before reassigning a device to ​another end user before sending a device out for repair or ​as a last resort when troubleshooting a misbehaving device. ​Don't forget a factory reset will remove all data apps and ​customization from the device. ​Make sure that anything you don't want to lose has been backed up or ​sync to the cloud. ​Another heads up watch out for expansion storage. ​Additional storage devices like SD cards or USB drives can contain personal or ​proprietary data doing a factory reset while expansion storage is attached ​might erase data that you intend to keep. 

- Maybe the mobile device won't boot or ​doesn't have a good enough data connection to download the update itself. ​In these cases, ​you can re flash or overwrite the OS of the device from a computer. ​But be careful pay close attention to the devices instructions for re flashing for ​some devices, re flashing will preserve the end user data on the device, but ​for others, the end result will be like a factory reset.

### Steps for reflash
1. Download the update to a computer

2. Attach the mobile device to a computer using a USB cable 

3. Run some software on the computer that will re-flash the mobile device 

## Troubleshooting Application Crashes

**System Logs**: Records of events and errors happening on a computer.

**Application Logs**: Records of events and errors related to applications.

**Event Viewer**: A Windows tool used to view and analyze system and application logs. Open it by typing `eventvwr.msc` in the Run box.

**Custom View**: A filter in Event Viewer that displays only the events you want to investigate.

**Error and Critical Events**: Log entries that can help identify application crashes and serious system problems.

**Timestamps**: Show when an event happened and help match errors to the time a crash occurred.

### Troubleshooting Steps

1. Identify whether the problem affects one computer, multiple computers, one user, or multiple users.
2. Check whether the problem is related to a specific application.
3. Open Event Viewer and examine the system and application logs.
4. Filter for **Error** and **Critical** events.
5. Check timestamps and error messages to find the root cause.
6. Try possible solutions until the problem is fixed.
7. Document the solution and share it with your team.

**Root Cause**: The underlying reason a problem occurs.

**Documentation**: Recording problems and their solutions so others can fix similar issues faster.

## Windows Troubleshooting Tools

**Windows Update**: Installs Windows updates, security fixes, and drivers.

**OEM Updates**: Updates from the hardware manufacturer's website, including drivers and firmware.

**Optimize Drives (Disk Defragmenter)**: Reorganizes fragmented files on hard drives to improve performance.

**Disk Cleanup**: Removes temporary and unnecessary files to free up disk space.

**CHKDSK**: Scans drives for bad sectors and attempts to recover readable data.

**Disk Management**: Manages drives, partitions, and drive letters.

**Event Viewer**: Displays system, hardware, and application errors and events.

**Registry Editor (`regedit`)**: Changes advanced Windows settings. Incorrect changes can cause serious problems.

**System Configuration (`msconfig`)**: Changes startup settings and services to help troubleshoot problems.

**Safe Mode**: Starts Windows with a limited set of drivers and services to help identify problems.

**System Troubleshooter**: Windows 11 tool for diagnosing and fixing problems with devices, networks, audio, and more.

## Common Windows Problems

**Slow Computer**: Restart the computer, check RAM and disk space, install updates, scan for malware, and check Event Viewer for errors.

**Frozen Computer**: Restart the computer and check Event Viewer for errors if the problem continues.

**Blue Screen (BSOD)**: Record the error code, restart the computer, and check Event Viewer for clues about the cause.

**Hardware Problems**: Check Device Manager, update drivers, and review system logs.

**Software Problems**: Update the software and check application logs for errors.

**Frozen Application**: End the application's process in Task Manager, then restart it.

**Peripheral Problems**: Check power, cables, USB ports, and Bluetooth connections. Check Device Manager if the device still doesn't work.

**Audio Problems**: Check volume, cables, sound settings, audio drivers, and the default audio device.

## Important Troubleshooting Tips

* **Restart First**: Restarting can resolve many common computer problems.
* **Check Logs**: Use Event Viewer to identify errors and possible causes.
* **Update Software**: Install Windows, driver, and application updates.
* **Research Error Codes**: Search error codes to find possible solutions.
* **Test One Thing at a Time**: Isolate possible causes to identify the problem.
* **Document Solutions**: Record fixes so similar problems can be solved faster in the future.

## Troubleshooting a Full Hard Drive

**Primary Hard Drive**: The drive where the operating system (OS) is installed.

**Low Disk Space**: When a drive has very little free storage, which can cause slow performance, crashes, and failed updates.

**Storage Sense**: Windows tool that automatically removes unnecessary files, such as temporary files and items in the Recycle Bin.

**Disk Cleanup**: Windows tool that removes temporary and unnecessary files to free up storage space.

**Windows Update Reset**: Troubleshooting tool that checks and repairs problems with Windows Update.

**Cloud Storage**: Stores files online, such as OneDrive or Google Drive, instead of only on your computer.

**Network Storage**: Storage accessed through a network, such as NAS or SAN.

**Online-Only Files**: Cloud files that don't take up local storage space until downloaded.

### Steps to Fix Low Disk Space

1. **Check free space**: See how much storage is available on the primary hard drive.
2. **Delete unnecessary files**: Use Storage Sense or Disk Cleanup.
3. **Reset Windows Update**: Fix potential update problems.
4. **Move files**: Transfer files to an external drive, network storage, or cloud storage.
5. **Set cloud files to online-only**: Reduce local storage usage.
6. **Uninstall unused apps**: Free up additional space.
7. **Scan for malware**: Viruses and malware can fill a hard drive with unwanted data.
8. **Reinstall Windows**: As a last resort, wipe the drive and reinstall the OS if other solutions fail.

**Important**: Regularly clean up hard drives and monitor free space to prevent performance problems and failed updates.

### What is disk cloning used for
- To image a computer system
- To back up a machine