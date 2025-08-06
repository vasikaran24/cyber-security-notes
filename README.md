BOLT

a hero is unleashed


It is useful to get familiar with the Bolt CMS and how it can be exploited using Authenticated Remote Code Execution

TASK 1:
-------

start the machine.

Ready to solve the challenge

Go ahead!

What port number has a web server with a CMS running?

TASK 2:
-------

open VM and go to NMAP and scan the ip address they provided


<img width="1100" height="162" alt="image" src="https://github.com/user-attachments/assets/bd7c8058-9da2-4026-b887-e593e2584e0a" />

ANSWER :8000


What is the username we can find in the CMS?

HTTP and HTTPS port is running so we  can access web site ,


<img width="2708" height="1302" alt="image" src="https://github.com/user-attachments/assets/f43ce52b-3aea-46c1-a1df-a476c52a4964" />

let's explore the website , 

<img width="1100" height="752" alt="image" src="https://github.com/user-attachments/assets/2915503a-db19-4dcc-afca-49e1d78036eb" />

we get the message from the admin (jake) and this user name bolt


ANSWER : Bolt

GO to the second article and we get the password we want


<img width="1100" height="687" alt="image" src="https://github.com/user-attachments/assets/3a509c2a-fe07-4453-b0df-36fdb1e1865e" />

GO to the second article and we get the password we want

ANSWER : boltadmin123

What version of the CMS is installed on the server? (Ex: Name 1.1.1)

<img width="1100" height="278" alt="image" src="https://github.com/user-attachments/assets/562186b4-215d-4239-8c2f-a91bd361ddca" />

 I go to the google and search for  boltCMS login page 
 I got it.

 As we have the username and password .so , try to login with the credentials we have 

 <img width="1100" height="561" alt="image" src="https://github.com/user-attachments/assets/ffd9110b-3495-4541-bbb4-8ce94288f80e" />

once we login ,we  get the dashboard of the  boltCMS and its version


There's an exploit for a previous version of this CMS, which allows authenticated RCE. Find it on Exploit DB. What's its EDB-ID?


GO to GHDB and search for the vulnerabilty and here it is , 

<img width="1100" height="418" alt="image" src="https://github.com/user-attachments/assets/c759a642-1b9b-4c5f-86a4-bd6644639f0b" />

ANSWER :48296

Metasploit recently added an exploit module for this vulnerability. What's the full path for this exploit? (Ex: exploit/....)

Note: If you can't find the exploit module its most likely because your metasploit isn't updated. Run `apt update` then `apt install metasploit-framework`

we can use in two ways .one is default available in our kali linux go and search " metasploit - framework "  or install using command " apt install metasploit-framework "

Using msf find the vulnerabilty 

<img width="1100" height="185" alt="image" src="https://github.com/user-attachments/assets/1a79e820-85fa-4cc9-8a1d-d1fef12122e1" />

ANSWER :exploit/unix/webapp/bolt_authenticated_rce

Use the module, and it can be seen that we need a username, password, rhost, and rhost to run this exploit

<img width="1100" height="633" alt="image" src="https://github.com/user-attachments/assets/80e6c8db-3cec-4126-b27c-2e35c938b481" />

 
Set username, password, rhost, and rhost with existing information.

<img width="1100" height="235" alt="image" src="https://github.com/user-attachments/assets/ef223d28-5918-4c06-bb9a-e1491847e42e" />

run the exploit 

<img width="1100" height="309" alt="image" src="https://github.com/user-attachments/assets/d794f9f3-e0c0-41e1-b621-ec4ad426571b" />

look for the flag in the machine

<img width="996" height="132" alt="image" src="https://github.com/user-attachments/assets/e3906923-625b-46c7-b8c6-9a469f3ed117" />

ANSWER :THM{wh0_d035nt_l0ve5_b0l7_r1gh7?}

In this article we have completed the “bolt” room on tryhackme. 

I made this article for my documentation in learning cybersecurity.











