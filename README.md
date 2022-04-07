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
 - Succesfully installed mysql and php.
 - Created a root web  directory file and open a new configuration file using  nano terminal editor. Though nano was a bit hard to use compared to vi i opted to edit the file using vi editor to add configuration details to my file.
     ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/php1.PNG)
 -  Activated my configuration file and tested Nginx  to check for any errors using this command `sudo nginx -t` which was a success.
      ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/php2.PNG)
 - Open my browser to check if LEMP stack was fully configured using my public Ip Address.
     ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/php4.PNG)
 - Tested php with nginx by creating a info.php file then deleted it.
 
  
 **Step 4: Retrieving data from MYSQL database using PHP **
 - Logged in to mysql console and  created a database(example_database) then created a user(example_user) and granted full privilleges on the database i created.
 - Created a test table and inserted data to it .
 - Created a php script to connect to mysql database and queries the contents of my test table.
   ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/mysqldb2.PNG)
   ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/mysqldb3.PNG)
   ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/mysqldb4.PNG)
   ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/mysqldb5.PNG)
   ![alt text](https://github.com/Ellawangari/DevOps-Project002/blob/main/Images/mysqldb6.PNG)
   
   
  ** This Project was an awesome learning experience as working on it was a bit fast due to earlier gained knowledge.**
 

**End of DevOps Project 2**

To try this project  [darey.io](https://www.darey.io) have a free trial to which you can practice this project.

