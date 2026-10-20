### System Administration
The field in IT that's responsible for maintaining reliable computer systems in a multi-user environment 

- **IT infrastructure** encompasses the software, the hardware, network, an services required for an organization to operate in an enterprise IT environment 

### Some PossibleJob titles for system admins are...
- Network admin
- Database admin

In some cases sys admins are responsible for maintaining all the company's servers

### Server
Software or a machine that provides services to other software or machines 

### KVM Switch
A device that lets you control multiple computers using one keyboard, monitor, and mouse.

### Data Center 
A facility that stores hundreds, if not thousands of servers 

- Best way to solve a problem is troubleshooting which is asking questions, isolating the problem, ​following the cookie crumbs and ​reading logs are the best ways to figure out the issue.

- It's super important to make sure that your company's data is routinely backed up ​somewhere preferably far away from its current location. 

- Avoid using administrator rights for tasks that don't require them, think before you type! The more you can do with admin rights the more you can mess up. Reverting to the previous stats is called rollback and some commands are easier to rollback then others so before you make a change think about the roll back and backup anything that you plan on deleting or changing.

## Recording System Administration Sessions

- **Documentation:** Planning changes before making them and recording the actions taken.
- **Ticketing System:** A system used to track problems, commands executed, and their outputs.
- **script:** A Linux command that records terminal commands and their output to a file.
  - Example: `script session.log`
  - Type `exit` or press `Ctrl+D` to stop recording.
- **ANSI Format:** A text format that can include terminal colors and formatting.
- **ansi2txt:** Converts ANSI-formatted output into plain text.
- **ansi2html:** Converts ANSI-formatted output into HTML.
- **Start-Transcript:** A PowerShell command that records commands and their output to a text file.
  - Example: `Start-Transcript -Path C:\Transcript.txt`
  - Use `Stop-Transcript` to stop recording.
- **Graphical Session Recording:** Recording actions performed through a graphical user interface (GUI).
- **OBS:** A tool that can record screen activity.
- **VLC:** A media player that can also record screen activity.
- **recordMyDesktop:** A Linux tool used to record desktop activity.

### Production
The parts of the infrastructure where a certain service is executed and served to its users

### Test environment 
A virtual machine running the same configuration as the production environment, but isn't actually serving any users of the service

### Secondary or Stand-by machine
This machine will be exactly the same as a production machine, but won't receive any traffic from actual users until you enable it to do so
 - firs, apply the changes to the secondary machine
 - Once the changes have been applied, make the stand-by machine the primary machine, and then apply the changes to the other machine 
 - for even bigger services, when you have lots of servers providing the service, you may want to have canaries meaning test it on a subset of machines to see if there is a problem. That way if there is a problem the issue only hits some of the users instead of all of them.


 - In general, the more users your services reaches, the more you'll want to ensure that changes aren't disruptive. The more important your services is to your company's operations, the more you'll work to keep the service up

 Let's say you're dealing with a problem ​either because you've found it ​or someone reported to you. ​Before you start fixing it, ​make sure you can recreate ​the error as you'll want to test ​your solution to make sure the problem ​is gone after you apply the fix. ​This is called a reproduction case

 ### Reproduction case
 Creating a road map to retrace the steps that led the user to an unexpected outcome

### ​When looking for a reproduction case, ​there are three questions you will need to answer. 

1. What steps did you take to get to this point?
2. what's the unexpected (bad) result?
3. what's the expected result?

### Scenario example of a reproduction case 
Let's say that you're trying to fix a problem where ​a user can't access a website page. ​The reproduction case would be ​navigating to the failing site with a web browser. ​The bad result is an error page, ​while the expected result is a visible website. ​Once you have the steps you need to recreate ​the unexpected result and ​you know what the right results should be, ​you can try to fix the underlying issue. 

- Remember always do this in your test instance never in production.and make sure to document all your findings

- After applying your fix, retrace the same steps that took you to the bad experience, if your fix worked, the expected experience should now take place 

## Cloud Services and System Administrators

- **Cloud Services:** Services that let companies use computing resources over the internet instead of managing all their own physical hardware.
- **Cloud Provider:** A company that manages cloud infrastructure, including physical servers and hardware.
- **On-Premises:** Hardware and servers physically located and managed at a company's own location.
- **Hardware Management:** Cloud providers handle physical server maintenance, replacement, and retirement.
- **Reduced Hardware Responsibilities:** Using cloud services means system administrators have less physical hardware to manage.
- **System Administrator Responsibilities:** In the cloud, system administrators may focus more on managing cloud resources, user access, security, configurations, and troubleshooting instead of maintaining physical servers.