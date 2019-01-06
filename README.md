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
listing -l (long listing) -t(by timestamp),-h(human readable)
### alias 
create alias e.g. alias ls='ls --color=auto'
### useradd  userdel
add new user or delete existing user e.g -> useradd -m someuser
### tar
zip directory or files -cvf(create verbose file), -czvf(z-zip), other (cjvf) e.g -> tar -cvf t1.tar totest/

read content of tar e.g. -> tar -tzf t1.tar






