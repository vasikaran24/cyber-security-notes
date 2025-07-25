             <<<<<<   🧾 Basic Linux Commands Cheat Sheet   >>>>>>

    Learn the most useful Linux commands for daily use in the terminal.

    ====================================
    📁 Navigation & Directory Commands
    =====================================

pwd        Print the current directory path
ls	       List files and folders
ls-l       List with details (permissions, size, date)
ls -a	     List all, including hidden files
cd folder  Change directory to folder
cd ..	     Go up one level
cd ~	     Go to home directory
mkdir name	Create a new directory
rmdir name	Remove an empty directory

==================
📄 File Commands
==================
  
touch file.txt	   Create a new empty file
cat file.txt	     Show file contents
nano file.txt	     Edit file with Nano editor
cp file1 file2	   Copy file1 to file2
mv old new	       Move/rename file or directory
rm file.txt     	 Delete a file
rm -r folder/     	Delete a folder and its contents

=================
🔍 Search & Find
==================
find . -name file.txt	    Find file.txt in current folder and subfolders
grep "word" file.txt	    Search for “word” inside file.txt
grep -r "word" folder/	  Recursively search in a folder

=====================================
📦 Package Management (Ubuntu/Debian)
======================================

sudo apt update     	  Refresh package list
sudo apt upgrade	      Upgrade all packages
sudo apt install name 	Install a package
sudo apt remove name	   Remove a package

============================
🛠️ System & Process Commands
=============================

top	          Show real-time system processes
htop	        (Better version of top; needs to be installed)
ps aux	       View all running processes
kill PID	     Kill process by PID
df -h	        Show disk usage in human-readable form
free -h      	Show memory usage

==========================
🔐 Permissions & Ownership
===========================
chmod +x script.sh	    Make file executable
chmod 755 file	Set     specific permissions
chown user:group file	  Change file ownership

======================
📡 Networking Commands
=======================

ping google.com	       Check if you're connected to the internet
ip a	                 Show IP addresses
ifconfig	             (Similar to ip a, may require install)
netstat -tulpn	       Show open ports (use with sudo)
curl http://example.com	 Get contents of a webpage

===============================
⬆️ File Permissions Quick Chart
================================

r	               Read
w	               Write
x	               Execute
-rw-r--r--	     File permission example: owner can read/write, others can only read

===========================
🧹 Extra Helpful Commands
===========================
history	           Show your command history
clear	             Clear terminal screen
man command	       open the manual for any command (e.g., man ls)
alias ll='ls -la'	 Create a shortcut command
sudo	             Run a command with admin privileges

