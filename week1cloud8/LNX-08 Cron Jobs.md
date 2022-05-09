# [Subject]
[Give a short summary of the subject matter.]

## Key terminology
[Write a list of key terminology with a short description. To prevent duplication you can reference to previous excersizes.]

## Exercise
Create a Bash script that writes the current date and time to a file in your home directory.
Register the script in your crontab so that it runs every minute.
Create a script that writes available disk space to a log file in ‘/var/logs’. Use a cron job so that it runs weekly.



### Sources
[List your sources you used for solving the exercise]

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
Create a Bash script that writes the current date and time to a file in your home directory.

rolf@Nest-Ro-Sijtema:~/scripts$ nano timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ echo timebash.sh
timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ./timebase.sh
-bash: ./timebase.sh: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ ./timebash.sh
-bash: ./timebash.sh: Permission denied
rolf@Nest-Ro-Sijtema:~/scripts$ chmod u+x timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ls
random.sh  scriptstext.txt  timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ls-l
ls-l: command not found
rolf@Nest-Ro-Sijtema:~/scripts$ ls -l
total 12
-rwxrw-r-- 1 rolf rolf 189 May  6 12:27 random.sh
-rw-rw-r-- 1 rolf rolf  45 May  6 12:41 scriptstext.txt
-rwxrw-r-- 1 rolf rolf  17 May  6 13:05 timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ./timebash.sh
Fri May  6 13:09:38 UTC 2022
rolf@Nest-Ro-Sijtema:~/scripts$ nano timebash.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ./timebash.sh
Fri May  6 13:15:55 UTC 2022
./timebash.sh: line 3: /home/date.txt: Permission denied
rolf@Nest-Ro-Sijtema:~/scripts$ sudo ./timebash.sh
Fri May  6 13:16:23 UTC 2022
rolf@Nest-Ro-Sijtema:~/scripts$ cd home
-bash: cd: home: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ ../
-bash: ../: Is a directory
rolf@Nest-Ro-Sijtema:~/scripts$ cd /..
rolf@Nest-Ro-Sijtema:/$ ls
bin   dev  home  lib32  libx32  mnt  proc  run   snap  sys  usr
boot  etc  lib   lib64  media   opt  root  sbin  srv   tmp  var
rolf@Nest-Ro-Sijtema:/$ cd home
rolf@Nest-Ro-Sijtema:/home$ ls
date.txt  rolf
rolf@Nest-Ro-Sijtema:/home$ 
rolf@Nest-Ro-Sijtema:/home$ cat date.txt
Fri May 6 13:16:23 UTC 2022
rolf@Nest-Ro-Sijtema:/home$ 

Register the script in your crontab so that it runs every minute.

3uur besteed met het team niet opgelost, ook Tom gevraagd niet gelukt. 

het kost teveel tijd en deadline is verstreken. 

https://linuxize.com/post/cron-jobs-every-5-10-15-minutes/  deze link gaat over de puntjes welke de runtijd aangeeft, day minute week, hour.  krijg het helaas niet voor elkaar. 

