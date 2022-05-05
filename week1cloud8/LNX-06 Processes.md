# [Subject]Processes in Linux can be divided into three categories: Daemons, Services, and Programs.
A daemon runs in the background and is non-interactive. A Service responds to requests from programs. A service may be interactive. A program is run and used by users (e.g. Vim).

In order to connect to remote Linux machines (virtual or not), you can use ssh (secure shell). To make this connection to your machine possible, you’ll have to start the ssh service by starting the ssh daemon. Before ssh there was telnet, which basically does the same thing, except the connection is not encrypted, so it is not secure. In this exercise we will use telnet for the sake of not messing with our ssh connection, but it is not recommended for use.

A process is an instance of running code. All code is stored in files somewhere on the system. In order to find these files, Linux will look in the $PATH variable (more about that in a later exercise). Every process has its own PID (Process ID) number.


### Sources
https://www.javatpoint.com/linux-telnet-command
https://forum.lowyat.net/topic/346775

### Overcome challanges
weinig uitdaging daar het beperkt aantal commands zijn, wel moeite na het installeren om weer terug te komen bij de root.

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
end