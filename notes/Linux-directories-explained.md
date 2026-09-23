# Linux directories explained

_Video length: 4 min | Status: done_

## Goal

Understand the purpose of key top-level Linux directories and see them for real with `ls` and `cd`.

## Concepts involved

- Everything starts from a single root directory (`/`),a tree of directories branch out from there, each with a specific job
- `/home` — personal files, one home directory per user (e.g. `/home/rjdecosta`)
- `/etc` — "Extended Text Configurations," system config files; back these up before editing
- `/var` — variable/changing data: logs, mail, print jobs (`/var/log` shows system activity)
- `/usr` — installed software; `/usr/bin` = executables ("binaries"), `/usr/lib64` = libraries, `/usr/share` = shared resources like docs
- `/tmp` — temporary storage, periodically cleaned out, accessible to every user, never store anything important here
- `/root` — home directory for the root (superuser) account, not accessible to normal users
- `/boot` — kernel and boot files, rarely touched except when troubleshooting boot problems
- `/mnt` — temporary mount point for external storage (USB drives, network shares)
- `/run` — runtime state for currently-running programs/services (e.g. process IDs, sockets), recreated fresh on every boot and wiped on restart
- `/dev`, `/proc`, `/sys` — system internals, safe to ignore as a beginner

## Commands

```bash
# ls / — list contents of the root directory
$ ls /
```

```bash
# cd — with no options/arguments, takes you to your own home directory
$ cd
$ pwd
```

```bash
# ls /var/log — see what the system has been logging
$ ls /var/log
```

## Notes

if i press cd with a wrong directory,a error message shows up