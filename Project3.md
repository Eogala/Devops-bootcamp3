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
| 1  |Deploy three servers                                  |
| 2  | Set up static websites on two servers using Nginx.                         |
| 3  | Use two separate HTML files with distinct content. Deploy one file to each server's index.html location.                                         |
| 4  |Set up Nginx on the third server. It will act as a load balancer.        |
| 5  |Configure Nginx to load and balance traffic between two static websites.                      |
| 6  |Add the Nginx Load balancer IP to the DNS A record.                              |
| 7  |Try accessing the website. Every time you reload the website you should see a different index.html.
                     |
