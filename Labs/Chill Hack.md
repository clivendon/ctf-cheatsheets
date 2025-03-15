---
type: {notes/writeup}
tags: [{PLATFORM NAME/CTF NAME}, {box/challenge}, {linux/win}, {easy/medium/hard}, {services}, {cve-number}, {tooling}, {techniques}]
reference: {URL}
category: {blackbox/web/rev-engineering/rooting/coding/hardware/blockchain/misc/steg/etc}
title: "{BOX NAME}"
difficulty: {easy, medium, hard}
user-voted: {easy, medium, hard}
date: {YYYY-MM-DD}
author: {AUTHOR NAME}
contact: {AUTHOR CONTACT}
---

# Chill hack

Target IP = 10.10.
Tun0 IP = {VPN ATTACKER IP}

---

## Information Gathering

### Open Ports & Running Services

```sh
{COMMAND}


```

**OS:** {Linux/Win}

| Port # | Service           |     |
| ------ | ----------------- | --- |
| #      | {NAME  + VERSION} |     |
| #      | {NAME  + VERSION} |     |
| #      | {NAME  + VERSION} |     |
Anurodh told me that there is some filtering on strings being put in the command -- Apaar

## Confirmed Users
Apaar


## Output of the sudo -l command

Matching Defaults entries for www-data on ubuntu:
    env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User www-data may run the following commands on ubuntu:
    (apaar : ALL) NOPASSWD: /home/apaar/.helpline.sh
---




daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/var/run/ircd:/usr/sbin/nologin
gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
systemd-network:x:100:102:systemd Network Management,,,:/run/systemd/netif:/usr/sbin/nologin
systemd-resolve:x:101:103:systemd Resolver,,,:/run/systemd/resolve:/usr/sbin/nologin
syslog:x:102:106::/home/syslog:/usr/sbin/nologin
messagebus:x:103:107::/nonexistent:/usr/sbin/nologin
_apt:x:104:65534::/nonexistent:/usr/sbin/nologin
lxd:x:105:65534::/var/lib/lxd/:/bin/false
uuidd:x:106:110::/run/uuidd:/usr/sbin/nologin
dnsmasq:x:107:65534:dnsmasq,,,:/var/lib/misc:/usr/sbin/nologin
landscape:x:108:112::/var/lib/landscape:/usr/sbin/nologin
pollinate:x:109:1::/var/cache/pollinate:/bin/false
sshd:x:110:65534::/run/sshd:/usr/sbin/nologin
aurick:x:1000:1000:Anurodh:/home/aurick:/bin/bash
mysql:x:111:114:MySQL Server,,,:/nonexistent:/bin/false
apaar:x:1001:1001:,,,:/home/apaar:/bin/bash
anurodh:x:1002:1002:,,,:/home/anurodh:/bin/bash
ftp:x:112:115:ftp daemon,,,:/srv/ftp:/usr/sbin/nologin
## Exploitation

### {PORT } - {SERVICE NAME}

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}


```

{SCREENSHOTS}

---

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

> [!USER FLAG]
> {USER FLAG}

{SCREENSHOT}

---

## Privilege Escalation

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

> [!ROOT FLAG]  
> {ROOT FLAG}  

{SCREENSHOT}

---

## SUCCESS

---

### Conclusion

{SCREENSHOT FINAL SCREEN}

---

## TODO

[ ] Share on Twitter  
[ ] Revise notes + Links to Notebook  
[ ] Export to HTML  
[ ] Publish on Medium  
[ ] Convert to PDF  
[ ] Push on GitHub  