## Level 0 ✅ 

Successfully completed. I mamaged to log in via ssh to the overthewire as bandit user via my terminal.

ssh bandit0@bandit.labs.overthewire.org -p 2220

#### Notes 
Port 2220 is typically used for Secure Shell (SSH) traffic, which enables users to securely access and manage remote systems and devices over a network. It is a common port used for SSH connections, particularly in cases where the default SSH port (22) has been blocked or restricted.

## Level 0 - Level 1 ✅ 

i used ls command to look what files are included and cat to read the readme.txt

passowrd for @bandit1 - **ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If**

Hooray ... Now im @bandit1 user.

i tried to login directly from bandit0 user to bandit1 without logging out from that session and it failed. it tuened out that, we had to logout from one ssh session to log into other one cuz server does not allow us to ssh from ssh session directly. 

## Level 1 - Level 2 ✅ 

This is quite interesting.... 

as bandit1 user ... via ls there was a file named - ... yep just -
then i tried to cat it. but nope, its not working.
then i tried to know what its filetype and hey, its not working either.

i dig up ... 

The issue is, usually - means a command/opertor thing on unix/linux. like a i/o string or thing. 

so i found the solution that we have to specifically define the path to that file via ./ 

its like saying " hey ... this is where the file located and process it as shown in the path.

so the answer was

cat ./- 

and the password for level 2 was - **263JGJPfgU6LtdEvgfWU1XP5yac29mFx**

