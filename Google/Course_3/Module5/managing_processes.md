You can open task manger user the key shortcut CTRL-SHIFT-ESC

# ps -x
allows you to see what processes are running on CLI
### Common status you will see
- R: running
- T: stopped
- S: interruptible sleep

### Signal
A way to tell a process that something's just happened 

### Process Explorer 
A Utility in Microsoft created to let IT Support Specialists, system admins, and other users look at running processes

# Linux Signals

Signals are messages sent to running processes to tell them to do something.

* **SIGTERM** — Asks a process to stop gracefully. The process has a chance to clean up before exiting.

  ```bash
  kill -TERM <PID>
  ```

* **SIGKILL** — Immediately kills a process. The process cannot catch or ignore this signal.

  ```bash
  kill -KILL <PID>
  ```

  or

  ```bash
  kill -9 <PID>
  ```

* **SIGTSTP** — Temporarily pauses/suspends a process. It does not kill the process. Pressing `Ctrl + Z` usually sends SIGTSTP.

  ```bash
  kill -TSTP <PID>
  ```

### Easy way to remember

```text
SIGTERM → Stop gracefully 🛑
SIGKILL → Kill immediately 💀
SIGTSTP → Pause temporarily ⏸️
```


