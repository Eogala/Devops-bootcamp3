# Project 3: Setup Load Balancing for Static Website Using Nignx
This project aims to teach Layer 7 load balancing and load balancing algorithms using Nginx as a Load Balancer.

## Type of Load Balancer
This is a reverse proxy load balancer configuration in Nginx, where Nginx acts as an intermediary for requests from clients seeking resources from the servers behind it. It's capable of distributing traffic across the servers listed in the upstream block.
## Characteristics
HTTP Load Balancing: This configuration balances HTTP requests.
Round Robin: By default, Nginx uses a round-robin algorithm to distribute traffic evenly among the servers unless otherwise specified.
Scalability: You can add more servers in the upstream block to scale out your application.

Tasks                                                                   |
|----|---------------------------------------------------------------------------------|
| 1  |Deploy three servers                          
        |
| 2  | Set up static websites on two servers using Nginx.         
                |
| 3  | Use two separate HTML files with distinct content. Deploy one file to each server's index.html location.                                         |
| 4  |Set up Nginx on the third server. It will act as a load balancer.     
   |
| 5  |Configure Nginx to load and balance traffic between two static websites.      
                |
| 6  |Add the Nginx Load balancer IP to the DNS A record.        
                      |
| 7  |Try accessing the website. Every time you reload the website you should see a different index.html.
                     |


Checklist
 - Task 1: Deploy three servers.
 - Task 2: Set up static websites on two servers using Nginx.
 - Task 3: Make a small change in the index.html file of one of the websites to differentiate between two servers OR  For a clearer distinction, use two separate HTML files with distinct content.
 - Task 4: Set up Nginx on the third server. It will act as a load balancer.
 - Task 5: Configure Nginx to load and balance traffic between two static websites.
 - Task 6: Add the Nginx Load balancer IP to the DNS A record.
 - Task 7: Try accessing the website. Every time you reload the website you should see a different index.html.
 
 # Documentation 
 Project1 was used as  guidance on spinning up an Ubuntu server, as well as creating and associating an elastic IP address with your server, among other tasks.

 3 ubuntu servers was spinned up

 ![pic](img)

## Install Nginx and Setup Your Website

Website template  was downloaded from your www.tooplate.com

Right click and select Inspect from the drop down menu

 ![pic](img)

![pic](img)

 ![pic](img)

 ![pic](img)

* To install Nginx, execute the following commands on your terminal.
sudo apt update

sudo apt upgrade

sudo apt install nginx

* Start your Nginx server by running the sudo systemctl start nginx command, enable it to start on boot by executing sudo systemctl enable nginx, and then confirm if it's running with the sudo systemctl status nginx command.

![pic](img)
