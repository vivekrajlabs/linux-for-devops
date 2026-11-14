# Lab 01: What is Linux, and your first commands

📺 Watch first: **Linux for DevOps #1** on [youtube.com/@vivekrajlabs](https://www.youtube.com/@vivekrajlabs) (English / हिंदी)

**Time:** 15 minutes · **You need:** any Ubuntu terminal ([setup](../setup.md))

**By the end you can:** read the prompt, run your first commands, and get help without Google.

---

## Scenario

It's day one at your new job. Your lead gives you access to a server and says: *"Find out which user you are, which
machine this is, which Linux it runs, and how long it has been up. Send me the answers."*

---

## Tasks

### Task 1: Read your prompt
Open your terminal. Look at the line before the cursor, for example `vivek@devops:~$`.
Write down the four parts: **who** you are, **which machine**, **where** you are, and what the last character means.

### Task 2: Who am I?
```bash
whoami
```
❓ Does the output match the first part of your prompt?

### Task 3: Which machine?
```bash
hostname
```
❓ Does it match the part after `@` in your prompt?

### Task 4: What time is it on the server?
```bash
date
```
❓ Which time zone does the server use? (Look at the letters before the year.)

### Task 5: How long has it been running?
```bash
uptime
uptime -p
```
❓ What changed when you added the option `-p`? (Hint: *p* = pretty.)

### Task 6: Which Linux is this?
```bash
lsb_release -d
cat /etc/os-release
```
❓ Which distro and version are you on?

### Task 7: Case matters
```bash
Date
```
❓ Read the error. What does Linux suggest?

### Task 8: Get help without Google
```bash
date --help
man date
```
Inside `man`, use the arrow keys to scroll, type `/UTC` and press Enter to search, and press `q` to quit.

---

## 🧪 Challenge

Using only `date --help` or `man date` (no internet), print:

1. only **today's day name**, for example `Saturday`
2. the date in this format: `2026-11-14`
3. the current time in **UTC**

## 🎯 Interview questions

1. What is the difference between the **kernel** and the **shell**?
2. What is a Linux **distribution**? Name three and where each is used.
3. Why do most servers and containers run Linux?
4. In `ls -l /home`, which part is the command, which is the option, and which is the argument?

---

✅ Done? Compare with [solutions.md](solutions.md). Keep [cheatsheet.md](cheatsheet.md) handy.
Next: **Lab 02: Moving around** (coming with Episode 2).
