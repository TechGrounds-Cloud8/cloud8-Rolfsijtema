# [Subject]
[Give a short summary of the subject matter.]

## Key terminology
[Write a list of key terminology with a short description. To prevent duplication you can reference to previous excersizes.]

## Exercise
### Sources
https://www.javatpoint.com/linux-telnet-command
https://forum.lowyat.net/topic/346775

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results

**Start the telnet daemon**
rolf@Nest-Ro-Sijtema:~$ sudo apt update
Hit:1 http://security.ubuntu.com/ubuntu focal-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease
Hit:3 http://archive.ubuntu.com/ubuntu focal-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu focal-backports InRelease
Reading package lists... Done
Building dependency tree       
Reading state information... Done
3 packages can be upgraded. Run 'apt list --upgradable' to see them.
rolf@Nest-Ro-Sijtema:~$ sudo apt install telnetd -y
Reading package lists... Done
Building dependency tree       
Reading state information... Done
telnetd is already the newest version (0.17-41.2build1).
The following package was automatically installed and is no longer required:
  libfreetype6
Use 'sudo apt autoremove' to remove it.
0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded.

**Find out the PID of the telnet daemon**
● inetd.service - Internet superserver
     Loaded: loaded (/lib/systemd/system/inetd.service; enabled; vendor preset: e>
     Active: active (running) since Thu 2022-05-05 14:36:19 UTC; 34min ago
       Docs: man:inetd(8)
   Main PID: 8943 (inetd)
      Tasks: 1 (limit: 4623)
     Memory: 644.0K
        CPU: 106ms
     CGroup: /system.slice/inetd.service
             └─8943 /usr/sbin/inetd

 **Find out how much memory telnetd is using**
              Memory: 644.0K

**Stop or kill the telnetd process**
              ~
rolf@Nest-Ro-Sijtema:~$ 
rolf@Nest-Ro-Sijtema:~$ ps ax| grep telnet
   9683 pts/1    S+     0:00 grep --color=auto telnet
rolf@Nest-Ro-Sijtema:~$ 
