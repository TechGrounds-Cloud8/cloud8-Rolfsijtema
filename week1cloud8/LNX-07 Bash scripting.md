# [bash scripting]
directory script aanmaken, aan path toevoegen

Bash Shell Scripting Definition "Bourne Again Shell" 
Bash is a command language interpreter. It is widely available on various operating systems and is a default command interpreter on most GNU/Linux systems. 

Shell is a macro processor which allows for an interactive or non-interactive command execution. het verbind zich met systemen. 

Scripting
Scripting allows for an automatic commands execution that would otherwise be executed interactively one-by-one.

## Key terminology
Echo laat zien wat er in de $PATH variabele staat
LS list laat de inhoud van de directory zien. 
een plek maken voor veel gebruikte commands 
HTTPD install:  sudo apt update  dan sudo apt install apache2
Run bash doe je met ./naam.sh
uitlezen: cat naam.txt 

## Exercise
Create a directory called ‘scripts’. Place all the scripts you make in this directory.
Add the scripts directory to the PATH variable.
Create a script that appends a line of text to a text file whenever it is executed.
Create a script that installs the httpd package, activates httpd, and enables httpd. Finally, your script should print the status of httpd in the terminal.

### Sources
bash scripting: https://www.youtube.com/watch?v=2hz7-v2f1sA
https://linuxize.com/post/how-to-install-apache-on-ubuntu-18-04/#

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
Create a directory called ‘scripts’. Place all the scripts you make in this directory.

rolf@Nest-Ro-Sijtema:~$ mkdir scripts
rolf@Nest-Ro-Sijtema:~$ ls
 rolf.txt  'sh rolf@18.196.32.244 -p55212 -i access_key.pe'  'ts... Done'
 scripts    techgrounds
rolf@Nest-Ro-Sijtema:~$ ls
 rolf.txt  'sh rolf@18.196.32.244 -p55212 -i access_key.pe'  'ts... Done'
 scripts    techgrounds
rolf@Nest-Ro-Sijtema:~$ echo scripts
scripts
rolf@Nest-Ro-Sijtema:~$ 
rolf@Nest-Ro-Sijtema:~$ type clear
clear is /usr/bin/clear
rolf@Nest-Ro-Sijtema:~$ 

Add the scripts directory to the PATH variable.

-bash: export: `/home/rolf/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin': not a valid identifier
rolf@Nest-Ro-Sijtema:~/scripts$ export PATH=/home/rolf/scripts:$PATH
rolf@Nest-Ro-Sijtema:~/scripts$ ls
rolf@Nest-Ro-Sijtema:~/scripts$ echo $PATH
/home/rolf/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
rolf@Nest-Ro-Sijtema:~/scripts$ 

Create a script that appends a line of text to a text file whenever it is executed.

rolf@Nest-Ro-Sijtema:~/scripts$ cat pandapunt.txt
cat: pandapunt.txt: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ cat "pandapunt.txt"
cat: pandapunt.txt: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ cd techgrounds
-bash: cd: techgrounds: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ cd techground
-bash: cd: techground: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ nano scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ ls
scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ cat scripttekst.txt
cat: scripttekst.txt: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ cat scriptstekst.txt
dit is de scripts tekstfile
rolf@Nest-Ro-Sijtema:~/scripts$ echo pandaontploft >> scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ cat scriptstekst.txt
dit is de scripts tekstfile
pandaontploft
rolf@Nest-Ro-Sijtema:~/scripts$ 

Create a script that installs the httpd package, activates httpd, and enables httpd. Finally, your script should print the status of httpd in the terminal.

result:
● apache2.service - The Apache HTTP Server
     Loaded: loaded (/lib/systemd/system/apache2.service; enabled; vendor preset: enabled)
     Active: active (running) since Fri 2022-05-06 09:11:02 UTC; 38s ago
       Docs: https://httpd.apache.org/docs/2.4/
   Main PID: 11330 (apache2)
      Tasks: 55 (limit: 4623)
     Memory: 5.6M
        CPU: 56ms
     CGroup: /system.slice/apache2.service
             ├─11330 /usr/sbin/apache2 -k start
             ├─11334 /usr/sbin/apache2 -k start
             └─11335 /usr/sbin/apache2 -k start

May 06 09:11:02 Nest-Ro-Sijtema systemd[1]: Starting The Apache HTTP Server...
May 06 09:11:02 Nest-Ro-Sijtema systemd[1]: Started The Apache HTTP Server.
rolf@Nest-Ro-Sijtema:~/scripts$ 

Create a script that generates a random number between 1 and 10, stores it in a variable, and then appends the number to a text file only if the number is bigger than 5. If the number is 5 or smaller, it should append a line of text to that same text file instead.

rolf@Nest-Ro-Sijtema:~/scripts$ echo $(( $RANDOM % 10 + 1 ))
2
rolf@Nest-Ro-Sijtema:~/scripts$ echo $(( $RANDOM % 10 + 1 ))
7
rolf@Nest-Ro-Sijtema:~/scripts$ 
rolf@Nest-Ro-Sijtema:~/scripts$ nano randomtekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ cat randomtekst.txt
hier worden nummers gemaakt

rolf@Nest-Ro-Sijtema:~/scripts$ mv randomtekst.txt random.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ls
random.sh  scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ chmod u+x random.sh
rolf@Nest-Ro-Sijtema:~/scripts$ echo random.sh
random.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ls
random.sh  scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ ls -l
total 8
-rwxrw-r-- 1 rolf rolf 28 May  6 09:28 random.sh
-rw-rw-r-- 1 rolf rolf 42 May  6 08:50 scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ 

rolf@Nest-Ro-Sijtema:~/scripts$ nano random.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ./sh
-bash: ./sh: No such file or directory
rolf@Nest-Ro-Sijtema:~/scripts$ ./random.sh
rolf@Nest-Ro-Sijtema:~/scripts$ ls
random.sh  scriptstekst.txt  scriptstext.txt
rolf@Nest-Ro-Sijtema:~/scripts$ cat scriptstext.txt
7
rolf@Nest-Ro-Sijtema:~/scripts$ rm scriptstekst.txt
rolf@Nest-Ro-Sijtema:~/scripts$ ls
random.sh  scriptstext.txt
rolf@Nest-Ro-Sijtema:~/scripts$ cat scriptstext.txt
7
rolf@Nest-Ro-Sijtema:~/scripts$ 
