# [Subject]
[Give a short summary of the subject matter.]

## Key terminology
aanmaken user met de juiste rechten

## Exercise
Create a new user in your VM.   useradd
The new user should be part of an admin group.  ??
The new user should have a password.
The new user should be able to use ‘sudo

### Sources
https://linuxize.com/post/how-to-create-users-in-linux-using-the-useradd-command/
https://linuxize.com/post/how-to-add-user-to-sudoers-in-ubuntu/

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
rolf@Nest-Ro-Sijtema:/$ sudo useradd panda2
rolf@Nest-Ro-Sijtema:/$ ls
bin  boot  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  snap  srv  sys  tmp  usr  var
rolf@Nest-Ro-Sijtema:/$ /etc/passwd
-bash: /etc/passwd: Permission denied
rolf@Nest-Ro-Sijtema:/$ sudo passwd panda2
New password: 
Retype new password: 
Sorry, passwords do not match.
passwd: Authentication token manipulation error
passwd: password unchanged
rolf@Nest-Ro-Sijtema:/$ sudo passwd panda2
New password: 
Retype new password: 
passwd: password updated successfully
rolf@Nest-Ro-Sijtema:/$ lost

Command 'lost' not found, did you mean:

  command 'last' from deb util-linux (2.34-0.1ubuntu9.3)
  command 'lout' from deb lout (3.39-3)
  command 'gost' from deb gost (0.1.0+git20181204.5afeda5e-1)
  command 'most' from deb most (5.0.0a-4)
  command 'host' from deb bind9-host (1:9.16.1-0ubuntu2.10)

Try: sudo apt install <deb name>

rolf@Nest-Ro-Sijtema:/$ sudo usermod -aG sudo pandapapa
rolf@Nest-Ro-Sijtema:/$ whoami
rolf
rolf@Nest-Ro-Sijtema:/$ sudo useradd pandamaster
rolf@Nest-Ro-Sijtema:/$ cdrom:x:24:
cdrom:x:24:: command not found
rolf@Nest-Ro-Sijtema:/$ floppy:x:25:
floppy:x:25:: command not found
rolf@Nest-Ro-Sijtema:/$ tape:x:26:
tape:x:26:: command not found
rolf@Nest-Ro-Sijtema:/$ sudo passwd pandamaster
New password: 
Retype new password: 
passwd: password updated successfully
rolf@Nest-Ro-Sijtema:/$ whoami
rolf
rolf@Nest-Ro-Sijtema:/$ sudo usermod -aG sudo pandamaster
rolf@Nest-Ro-Sijtema:/$ cat /etc/group

voice:x:22:
cdrom:x:24:
floppy:x:25:
tape:x:26:
sudo:x:27:rolf,pandamaster
audio:x:29:
dip:x:30:
www-data:x:33:
backup:x:34:
operator:x:37:
list:x:38:
irc:x:39:
src:x:40:
gnats:x:41:
shadow:x:42:
utmp:x:43:
video:x:44:
sasl:x:45:
plugdev:x:46:
staff:x:50:
games:x:60:
users:x:100:
nogroup:x:65534:
systemd-journal:x:101:
systemd-network:x:102:
systemd-resolve:x:103:
systemd-timesync:x:104:
crontab:x:105:
messagebus:x:106:
input:x:107:
kvm:x:108:
render:x:109:
syslog:x:110:
tss:x:111:
uuidd:x:112:
tcpdump:x:113:
ssh:x:114:
landscape:x:115:
admin:x:116:
netdev:x:117:
lxd:x:118:
systemd-coredump:x:999:
rolf:x:1000:
pandamaster:x:1003:
rolf@Nest-Ro-Sijtema:/$ cat etc/group | grep pandamaster
sudo:x:27:rolf,pandamaster
pandamaster:x:1003:
rolf@Nest-Ro-Sijtema:/$ cat etc/passwd | grep pandamaster
pandamaster:x:1003:1003::/home/pandamaster:/bin/sh
rolf@Nest-Ro-Sijtema:/$ 