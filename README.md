# DevOps-Project002
Second project from the guided [darey.io](https://www.darey.io) DevOps Engineer Scholarship 

****Project Implementation****
Technology Stack used was **LEMP**( Linux Nginx MYSQL PHP)

The first step and others which were similar to Project001.

**Step 1: Creating an AWS instance & Connecting to it using Mobaxterm**
- Downloaded my pem file to access my AWS Ubuntu server using Mobaxterm on my windows pc.
- Made the download folder as the persistent home directory since that's where my pem file was located.
- Added new inbound rules to connect to the instance using SSH.
- Once the inbound rules were all set I was now able to connect to my instance using the SSH on Mobaxterm.

**Step 2: Installing Nginx web server on my AWS instance**
-Connected to the AWS instance on Mobaxterm and installed Nginx.
- to update the server package index and install nginx  
 `sudo apt update`
`sudo apt install nginx`
- to verify nginx was installed   `sudo systemctl status nginx`
 ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/nginx1.PNG)
- Added an inbound rule to open port 80 and tested my nginx server from the web browser using my public IP address which was a success.
 ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/nginx2.PNG)
 
 **Step 3: Installing MYSQL ,PHP and configuring nginx to use PHP processor **
 
 
