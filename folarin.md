*Lecturer: Madu Valentine*
*CLOUD ENGINEERING ASSIGNMENT*
06:59 PM
.create a user
. set an expiry date of 2weeks for the user
. prompt the user to change there password on login
. attach the user to a group called altschool
. allow altschool group to be able to run only cat command on /etc/
. create another user. make sure that this user doesn't have a home directory.


**Cloud engineering assingment**


vagrant@ubuntu-jammy:~$ sudo useradd -m -s /bin/bash folarin
useradd: user 'folarin' already exists
vagrant@ubuntu-jammy:~$ sudo passwd folarin
New password:
Retype new password:
passwd: password updated successfully
vagrant@ubuntu-jammy:~$ sudo chage -E 2023-08-31 folarin
vagrant@ubuntu-jammy:~$ sudo chage -d 0 folarin
vagrant@ubuntu-jammy:~$ sudo usermod -aG altschool folarin
usermod: group 'altschool' does not exist
vagrant@ubuntu-jammy:~$ sudo groupadd altschool
vagrant@ubuntu-jammy:~$ sudo usermod -aG altschool folarin
vagrant@ubuntu-jammy:~$ sudo visudo
vagrant@ubuntu-jammy:~$ sudo visudo
visudo: /etc/sudoers.tmp unchanged
vagrant@ubuntu-jammy:~$ sudo visudo
vagrant@ubuntu-jammy:~$ sudo cat /etc/hostname
ubuntu-jammy
vagrant@ubuntu-jammy:~$ sudo visudo
vagrant@ubuntu-jammy:~$ sudo cat /etc/hostname
ubuntu-jammy
vagrant@ubuntu-jammy:~$ sudo useradd -M lekan
useradd: user 'lekan' already exists
vagrant@ubuntu-jammy:~$ sudo userdel john
userdel: user 'john' does not exist
vagrant@ubuntu-jammy:~$ sudo userdel lekan
vagrant@ubuntu-jammy:~$ sudo userdel Lekan
vagrant@ubuntu-jammy:~$ sudo useradd -M lekan
vagrant@ubuntu-jammy:~$

9

![screenshot]("C:\Users\ghost\Desktop\New folder (3)\assingment 1.jpg")
