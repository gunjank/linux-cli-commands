# linux-cli-commands
Important Linux CLI Commands 

### tty
display terminal device
### w
shows users logged in
### ctrl+l
clear screen
### cat /etc/shells 
show all available shells
### pwd 
print working directory 
### ls -a 
list all including hidden files
### history
list history of previously used commands 
### cat 
concatenate files(s) contents
### tac 
same as cat except print contents bottom to top
### head
show top contents of a file
### tail 
show bottom 10 or more lines if used with -f or -n (number of lines)
### less
page file contents - backwords or forward
### more 
page file contents forward 
### cut
display only needed columns , e.g. show fields 1 and 3 only-> cut -f1,3 -d":" /etc/passwd 
### sort
display sorted contents , e.g. sort column 3-> sort -k 3 -t":" /etc/passwd
### cut | sort
use certain column and then sort  e.g > cut -f1 -d":" /etc/passwd | sort 
### cp  and mv 
cp copy, mv move or rename.  -i(interactive) -R (recursive) -a (maintain original user access)
### rm 
cp copy, mv move or rename.  -i -rf (recursive)
### readlink
read source or target path for a link
### ls 
listing -l (long listing) -t(by timestamp),-h(human readable), -F (file type)
### alias 
create alias e.g. alias ls='ls --color=auto'
### useradd  userdel
add new user or delete existing user e.g -> useradd -m someuser
### tar
zip directory or files -cvf(create verbose file), -czvf(z-zip), other (cjvf) e.g -> tar -cvf t1.tar totest/

read content of tar e.g. -> tar -tzf t1.tar
untar or expand  e.g. -> tar -xzvf t2.tar.gz 
### find 
find matching file -newer (newer than)  e.g - >find . -newer test.sh  

find from a directory with matching name e.g. -> find /usr/share/ -name '*.pdf'

search and list with details {} is a placeholder e.g. -> find /usr/share/ -name '*.pdf' -exec ls -lh {} \;

search if size greater than 110k e.g. -> find /usr/share/ -size +100k

### > 
> write to file (create if not present)

>> append to a file (create if not available)

< read from a file

1> standard output or default

2> errors output 

set -o noclobber - prevents an existing file being overwritten

>| ignore noclobber

### mkfifo 
create named pipe e.g. -> mkfifo /tmp/somename
### tee 
send output to a file and to the screen at the same time e.g. -> ls /etc | tee out.txt 
### uptime
uptime for system and each user also load average (1 min, 5min, 15 min)
### grep 
search e.g grep -i (ignore case) Server(search word) /etc/ntp.conf (search in)

grep '\bserver\b' (setting boundry) 

grep '^server\b' (setting boundry and start of the line) 

grep -ve '^#' -ve '^$' '^server\b' (setting boundry and start of the line) 

