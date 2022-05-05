
You can view a file’s permissions by creating a long listing. A file’s permissions, as well as its owner and group, can be changed as well.
Any user listed in /etc/passwd can be assigned as owner of a file.
Any group listed in /etc/group can be assigned as the group of a file.

## Key terminology
[Write a list of key terminology with a short description. To prevent duplication you can reference to previous excersizes.]

## Exercise
Create a text file.
Make a long listing to view the file’s permissions. Who is the file’s owner and group? What kind of permissions does the file have?
Make the file executable by adding the execute permission (x).
Remove the read and write permissions (rw) from the file for the group and everyone else, but not for the owner. Can you still read it?
Change the owner of the file to a different user. If everything went well, you shouldn’t be able to read the file unless you assume root privileges with ‘sudo’.
Change the group ownership of the file to a different group.

### Sources
[List your sources you used for solving the exercise]

### Overcome challanges
duidelijk gemaakt voor mijzelf dat de positie vanuit waar je wat doet heel belangrijk is.  dit zorgt vaak voor problemen.  aanmaken en toewijzen sudo" moet vanuit ROOT user rolf

### Results
**Create a text file**
rrolf@Nest-Ro-Sijtema:/home$ cd rolf
rolf@Nest-Ro-Sijtema:~$ cd techgrounds
rolf@Nest-Ro-Sijtema:~/techgrounds$ nano pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandapunt.txt"
Dit is opdracht 5 LNX
het maken van een tekst en deze toewijzen aan alle panda's en ook de rechten aanpassen
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -lh
total 16K
-rw-rw-r-- 1 rolf rolf  96 May  4 14:47 clitekst.txt
-rw-rw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf  22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf  18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 
**Make a long listing to view the file’s permissions. Who is the file’s owner and group?**
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat /etc/passwd
root:x:0:0:root:/root:/bin/bash
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
systemd-network:x:100:102:systemd Network Management,,,:/run/systemd:/usr/sbin/nologin
systemd-resolve:x:101:103:systemd Resolver,,,:/run/systemd:/usr/sbin/nologin
systemd-timesync:x:102:104:systemd Time Synchronization,,,:/run/systemd:/usr/sbin/nologin
messagebus:x:103:106::/nonexistent:/usr/sbin/nologin
syslog:x:104:110::/home/syslog:/usr/sbin/nologin
_apt:x:105:65534::/nonexistent:/usr/sbin/nologin
tss:x:106:111:TPM software stack,,,:/var/lib/tpm:/bin/false
uuidd:x:107:112::/run/uuidd:/usr/sbin/nologin
tcpdump:x:108:113::/nonexistent:/usr/sbin/nologin
sshd:x:109:65534::/run/sshd:/usr/sbin/nologin
landscape:x:110:115::/var/lib/landscape:/usr/sbin/nologin
pollinate:x:111:1::/var/cache/pollinate:/bin/false
systemd-coredump:x:999:999:systemd Core Dumper:/:/usr/sbin/nologin
rolf:x:1000:1000::/home/rolf:/bin/bash
lxd:x:998:100::/var/snap/lxd/common/lxd:/bin/false
pandamaster:x:1003:1003::/home/pandamaster:/bin/sh
rolf@Nest-Ro-Sijtema:~/techgrounds$ 
**What kind of permissions does the file have?**
drwxrwxr-x 2 rolf rolf 4096 May  5 09:36 .
drwxr-xr-x 6 rolf rolf 4096 May  4 13:33 ..
-rw-rw-r-- 1 rolf rolf   96 May  4 14:47 clitekst.txt
-rw-rw-r-- 1 rolf rolf  109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf   22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf   18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls a
ls: cannot access 'a': No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -lh pandapunt.txt
-rw-rw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 

drwxrwxr-x 2 rolf rolf 4096 May  5 09:36 .
drwxr-xr-x 6 rolf rolf 4096 May  4 13:33 ..
-rw-rw-r-- 1 rolf rolf   96 May  4 14:47 clitekst.txt
-rw-rw-r-- 1 rolf rolf  109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf   22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf   18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls a
**Make the file executable by adding the execute permission (x).**
ls: cannot access 'a': No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -lh pandapunt.txt
-rw-rw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ chmod u+x pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf  96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf  22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf  18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo groupadd panditos
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf  96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf  22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf  18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chgrp panditos pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf      96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 
-rw-rw-r-- 1 rolf rolf  96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf  22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf  18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo groupadd panditos
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
**Remove the read and write permissions (rw) from the file for the group and everyone else, but not for the owner. Can you still read it?**
-rw-rw-r-- 1 rolf rolf  96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf rolf 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf  22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf  18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chgrp panditos pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf      96 May  4 14:47 clitekst.txt
-rwxrw-r-- 1 rolf panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chown rolf pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo go-rw pandapunt.txt
sudo: go-rw: command not found
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chmod go-rw pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf      96 May  4 14:47 clitekst.txt
-rwx------ 1 rolf panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 
**Change the owner of the file to a different user. If everything went well, you shouldn’t be able to read the file unless you assume root privileges with ‘sudo'**

rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandapunt" 
cat: pandapunt: No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandapunt.txt" 
Dit is opdracht 5 LNX
het maken van een tekst en deze toewijzen aan alle panda's en ook de rechten aanpassen
rolf@Nest-Ro-Sijtema:~/techgrounds$ chmod u-r pandapunt.txt 
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf rolf      96 May  4 14:47 clitekst.txt
--wx------ 1 rolf panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandapunt.txt"
cat: pandapunt.txt: Permission denied
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo cat "pandapunt.txt"
Dit is opdracht 5 LNX
het maken van een tekst en deze toewijzen aan alle panda's en ook de rechten aanpassen
rolf@Nest-Ro-Sijtema:~/techgrounds$ 

**Change the owner of the file to a different user. If everything went well, you shouldn’t be able to read the file unless you assume root privileges with ‘sudo’**
-rw-rw-r-- 1 rolf rolf      96 May  4 14:47 clitekst.txt
--wx------ 1 rolf panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandapunt.txt"
cat: pandapunt.txt: Permission denied
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo cat "pandapunt.txt"
Dit is opdracht 5 LNX
het maken van een tekst en deze toewijzen aan alle panda's en ook de rechten aanpassen
rolf@Nest-Ro-Sijtema:~/techgrounds$ chown rwx pandamaster pandapunt.txt
chown: invalid user: ‘rwx’
rolf@Nest-Ro-Sijtema:~/techgrounds$ chown pandamaster pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chown pandamaster pandatext.txt
chown: cannot access 'pandatext.txt': No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chown pandamaster pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf        rolf      96 May  4 14:47 clitekst.txt
--wx------ 1 pandamaster panditos 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf        rolf      22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf        rolf      18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 

**Change the group ownership of the file to a different group**
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "pandamaster2"
cat: pandamaster2: No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chgrp pandamaster2 pandapunt.txt 
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf        rolf          96 May  4 14:47 clitekst.txt
--wx------ 1 pandamaster pandamaster2 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf        rolf          22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf        rolf          18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ sudo chmod go+rw pandapunt.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls -l
total 16
-rw-rw-r-- 1 rolf        rolf          96 May  4 14:47 clitekst.txt
--wxrw-rw- 1 pandamaster pandamaster2 109 May  5 09:36 pandapunt.txt
-rw-rw-r-- 1 rolf        rolf          22 May  4 12:07 rolftekst
-rw-rw-r-- 1 rolf        rolf          18 May  4 14:52 techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 



