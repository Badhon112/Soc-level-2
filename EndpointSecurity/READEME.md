## Processes

- _Running instances of programs and applications_
  - Partitioned set of system resources (CPU, memory, I/O)
- _System (Windows) Processes_
  - OS core functions
  - System, smss.exe, csrss.exe
- _User (Application) Processes_
  - Initiated by users
  - chrome.exe, notepad.exe, minesweeper.exe
- _Service (Background) Processes_
  - Background Functions
  - Windows Update, Print Spooler, Lsass,exe

- _In The Windows CMD_

```bash
$ tasklist
$ tasklist /V
$ tasklist /M
$ tasklist /M /FI
$ tasklist /M /FI "PID eq 2088" /M
$ netstat -anob
$ tasklist /FI "IMAGENAME eq notmalware.exe"
# DLL = Dynamic Link Library
$ wmic
# wmic = Windows Management Instrumentation Command Line
$ wmic process where processid=id get name, parentprocessid, processid
```

- In the Linux

```bash
$ nc -lnvp 3333

```

---

