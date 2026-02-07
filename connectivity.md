#### Secure copy: 

The scp (secure copy) command in Linux systems is used to copy file(s) between servers in a secure way. 
The SCP command, or secure copy, allows the secure transfer of files between the local host and the remote host or between two remote hosts. It uses the same authentication and security as is used in the Secure Shell (SSH) protocol. SCP is known for its simplicity, security, and pre-installed availability.

If you want to copy data or a file from your local computer to the Linux server, first you need to copy the public key of your local computer to your Linux server
Then check if you will be able to connect or not.

1. Windows to a virtual server
```
scp docker-key.pem ubuntu@3.140.240.229:/home/ubuntu (apply on Windows)
scp -i "aws_login.pem" handtime-html.zip ubuntu@ec2-18-191-102-60.us-east-2.compute.amazonaws.com:/home/ubuntu
```
2. Virtual to Windows 
```
scp -i "linux.pem" ubuntu@13.58.119.184:/home/ubuntu/ubuntu-backup C:\Users\91916\Downloads
```
