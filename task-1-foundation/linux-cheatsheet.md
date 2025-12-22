# Linux Cheat-Sheet (Cybersecurity Basics)

## File System Navigation
pwd                 - show current working directory  
ls                  - list files  
ls -la              - list files with permissions  
cd <directory>      - change directory  
cd ..               - go back one directory  
tree                - show directory structure  

## File & Directory Management
touch file.txt      - create empty file  
mkdir folder        - create directory  
rm file.txt         - delete file  
rm -r folder        - delete directory  
cp file1 file2      - copy file  
mv file1 file2      - move or rename file  

## File Viewing
cat file.txt        - display file content  
less file.txt       - view file page by page  
head file.txt       - show first lines  
tail file.txt       - show last lines  

## File Permissions
chmod 777 file      - full permissions  
chmod 755 file      - owner full, others read/execute  
chmod 644 file      - standard file permission  
chown user:user file - change file owner  

## User & System Info
whoami              - current user  
id                  - user ID info  
uname -a            - system information  
hostname            - system hostname  

## Package Management
apt update          - update package list  
apt upgrade         - upgrade packages  
apt install <pkg>   - install package  
apt remove <pkg>    - remove package  
dpkg -l             - list installed packages  

## Networking Commands
ip a / ifconfig     - show IP address  
ping <ip/host>      - test connectivity  
netstat -tuln       - list open ports  
ss -tuln            - socket statistics  
traceroute <host>   - trace network path  

## Process Management
ps aux              - list running processes  
top                 - real-time process monitor  
kill <pid>          - terminate process  

## Disk & Memory
df -h               - disk usage  
du -sh <dir>        - directory size  
free -h             - memory usage  

## Archives & Compression
tar -cvf file.tar dir/   - create tar  
tar -xvf file.tar        - extract tar  
zip file.zip file        - create zip  
unzip file.zip           - extract zip  

## Logs & History
history             - command history  
clear               - clear terminal  

## Useful Security Commands
sudo                - run command as root  
grep "text" file    - search text  
find / -name file   - find files  

