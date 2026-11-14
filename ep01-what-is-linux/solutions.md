# Lab 01: Solutions

Try every task yourself first. Your output will differ (your username, machine name and time), and that's expected.

## Tasks

**Task 1.** For `vivek@devops:~$`: `vivek` is the **user**, `devops` is the **machine (hostname)**, `~` is the **current
folder** (your home, `/home/vivek`), and `$` means **ready for a command as a normal user**. If you see `#` instead,
you are **root**, the admin. Be extra careful there.

**Task 2.** `whoami` prints your username, the same as the first part of the prompt.

**Task 3.** `hostname` prints the machine name, the same as the part after `@`.

**Task 4.** The letters before the year are the time zone, for example `IST` or `UTC`. Servers often run in **UTC**, so
check this before you read log timestamps.

**Task 5.** `uptime` shows the time, how long the system has been up, logged-in users and the load average.
`uptime -p` prints only the "up" part in plain English, for example `up 3 days, 2 hours, 14 minutes`.

**Task 6.** For example `Description:	Ubuntu 24.04.1 LTS`. `/etc/os-release` holds the same information, with more fields
(`NAME`, `VERSION_ID`, `ID`…). Scripts read this file to detect the distro.

**Task 7.** Linux is **case-sensitive**: `Date` is not `date`. Ubuntu says something like
`Command 'Date' not found, did you mean: command 'date' from deb coreutils`.

**Task 8.** `--help` is a short summary; `man` is the full manual. `/word` searches, `n` jumps to the next match, `q` quits.

## Challenge

```bash
date +%A            # 1. Saturday
date +%F            # 2. 2026-11-14   (same as date +%Y-%m-%d)
date -u             # 3. time in UTC
```

`+FORMAT` is an **argument** that tells `date` how to print. You found the `%` codes in `man date`.
That's the skill: reading the manual instead of searching the internet.

## Interview answers (short versions)

1. **Kernel vs shell.** The kernel is the core of Linux: it talks to the hardware (CPU, memory, disk) and runs programs.
   The shell is a program that reads the commands you type and asks the kernel to run them. You → shell → kernel → hardware.
2. **Distribution.** The Linux kernel plus tools, a package manager and defaults, packaged together. Ubuntu (cloud and
   beginners), Red Hat / Rocky (enterprises and banks), Alpine (tiny, inside Docker images), Amazon Linux (AWS).
3. **Why servers run Linux.** Free and open source, stable for years without a reboot, everything is scriptable so it
   automates well, and containers (Docker, Kubernetes) are built on Linux kernel features.
4. **`ls -l /home`.** `ls` is the command (what to do), `-l` is the option (how: long format), and `/home` is the argument
   (what to do it on).
