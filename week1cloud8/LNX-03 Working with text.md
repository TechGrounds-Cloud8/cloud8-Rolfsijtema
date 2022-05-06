# [Subject]
Het oefen in het aanmaken van een input folder, en output,  tekst aanmaken en uitlezen. 


## Key terminology
[Write a list of key terminology with a short description. To prevent duplication you can reference to previous excersizes.]

## Exercise
### Sources
[List your sources you used for solving the exercise]

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results

rolf@Nest-Ro-Sijtema:~$ man sudo_root
rolf@Nest-Ro-Sijtema:~$ ls
rolf@Nest-Ro-Sijtema:~$ sudo ls
rolf@Nest-Ro-Sijtema:~$ ls
rolf@Nest-Ro-Sijtema:~$ mkdir techgrounds
rolf@Nest-Ro-Sijtema:~$ ls
techgrounds
rolf@Nest-Ro-Sijtema:~$ sudo su
root@Nest-Ro-Sijtema:/home/rolf# ls
techgrounds
root@Nest-Ro-Sijtema:/home/rolf# cat > rolf.txt I am a lost panda
cat: I: No such file or directory
cat: am: No such file or directory
cat: a: No such file or directory
cat: lost: No such file or directory
cat: panda: No such file or directory
root@Nest-Ro-Sijtema:/home/rolf# cat > rolf.txt
I am a lost panda

rolf@Nest-Ro-Sijtema:~$ cd techgrounds
rolf@Nest-Ro-Sijtema:~/techgrounds$ nano clitekst.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ car "clitekst.txt"

Command 'car' not found, but can be installed with:

sudo apt install ucommon-utils

rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "clitekst.txt"
Dit is de opdracht voor Cli
Er zijn 2 regels tekst hiervoor nodig
rolf@Nest-Ro-Sijtema:~/techgrounds$ echo hello world
hello world
rolf@Nest-Ro-Sijtema:~/techgrounds$ echo -n hello world
rolf@Nest-Ro-Sijtema:~/techgrounds$ echo "hello world" >> clitekst.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "clitekst"
cat: clitekst: No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls
clitekst.txt  rolftekst
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "clitekst"
cat: clitekst: No such file or directory
rolf@Nest-Ro-Sijtema:~/techgrounds$ ls
clitekst.txt  rolftekst
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "clitekst.txt"
Dit is de opdracht voor Cli
Er zijn 2 regels tekst hiervoor nodig
hello world
rolf@Nest-Ro-Sijtema:~/techgrounds$ echo "techground is top" >> clitekst.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "clitekst.txt"
Dit is de opdracht voor Cli
Er zijn 2 regels tekst hiervoor nodig
hello world
techground is top
rolf@Nest-Ro-Sijtema:~/techgrounds$ grep "techground" clitekst.txt
techground is top
rolf@Nest-Ro-Sijtema:~/techgrounds$ grep "techground" clitekst.txt >> techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ cl

Command 'cl' not found, but can be installed with:

sudo apt install cl-launch

rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "techgrounds.txt
> cat "techgrounds.txt"
> cd ..
> 
clitekst.txt     rolftekst        techgrounds.txt  
> -bash: unexpected EOF while looking for matching `"'
-bash: syntax error: unexpected end of file
rolf@Nest-Ro-Sijtema:~/techgrounds$ cat "techgrounds.txt"
techground is top
rolf@Nest-Ro-Sijtema:~/techgrounds$ cl

Command 'cl' not found, but can be installed with:

sudo apt install cl-launch

rolf@Nest-Ro-Sijtema:~/techgrounds$ ls
clitekst.txt  rolftekst  techgrounds.txt
rolf@Nest-Ro-Sijtema:~/techgrounds$ 
