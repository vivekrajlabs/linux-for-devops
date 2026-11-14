# Cheat sheet 01: First commands

| Command | Stands for | What it does | Example output |
|---|---|---|---|
| `whoami` | who am I | Your username | `vivek` |
| `hostname` | host name | The machine's name | `devops` |
| `date` | date | Date, time and time zone | `Sat Nov 14 10:30:12 IST 2026` |
| `date -u` | UTC | The time in UTC | `Sat Nov 14 05:00:12 UTC 2026` |
| `uptime -p` | pretty uptime | How long since the last restart | `up 3 days, 2 hours` |
| `lsb_release -d` | Linux Standard Base, description | Which distro and version | `Ubuntu 24.04.1 LTS` |
| `cat /etc/os-release` | concatenate (show) a file | Full distro details | `NAME="Ubuntu"` … |
| `<cmd> --help` | help | Quick usage summary | |
| `man <cmd>` | manual | The full manual: `/word` search, `n` next, `q` quit | |
| `clear` | clear | Clear the screen (or press `Ctrl+L`) | |

## Reading the prompt

```
vivek@devops:~$
  │     │    │ └─ $ = normal user, ready   (# = root, be careful)
  │     │    └─── ~ = where you are (home)
  │     └──────── machine name
  └────────────── your username
```

## Anatomy of a command

```
ls   -l      /home
│    │       └─ argument: what to do it on
│    └───────── option: how to do it
└────────────── command: what to do
```

## Golden rules

- Linux is **case-sensitive**: `Date` ≠ `date`.
- Stuck? `--help` first, then `man`.
- Never paste a command you don't understand.
