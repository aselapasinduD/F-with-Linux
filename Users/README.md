# User Related Commands

This section provides an overview of the most commonly used Linux commands, tailored for Linux-based systems. The majority of these commands have been tested on the Debian Linux distribution, ensuring reliability and compatibility.

## Handle Users

**Add Users:** User adding command.
```bash
sudo useradd <new-user-name>
```
**Add Users:** User adding with home folder command.
```bash
sudo useradd -m <new-user-name>
```
**Add User Password:** Give a password to the newly added user.
```bash
sudo passwd <newly-added-username>
```
**Switch Users** 
```bash
sudo su - <switch-user-name>
```
**List All Users:** Without format
```bash
cat /etc/passwd
```
**List All Users:** With format
```bash
awk -F: '{printf "%-20s%s\n", $1, $6}' /etc/passwd
```