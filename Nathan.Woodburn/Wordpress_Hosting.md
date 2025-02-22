# Wordpress Hosting

## Introduction
This project is to allow easy hosting of Wordpress websites on Handshake domains.  
It is likely to be a paid service (due to compute resources required), but the installation scripts will be available for free to allow anyone to host their own Wordpress server.  

## Features
- Easy setup scripts to allow easy expansion of the service  
One line command to install all the required software (Docker and nginx)

- Full admin control of the Wordpress server for the domain owner.

- Easy to assign wordpress servers  
  Probably via a discord bot with a license key to allow creation of the server.  
  API to create a license key when the user pays for the service. (optionally via ADMIN discord command)

- Full SSL support to allow secure connections to the Wordpress server


## Estimated project timeline
1. Finalise the Wordpress server setup script to remove any bugs that may be present. (1-2 hrs)
2. Create a script that takes in a license key and domain and will create a Wordpress server for that domain if the license key is valid. (1-2 hrs)
3. Update the HNSHosting discord bot to allow Wordpress hosting. (1-2 hrs)
4. Test the Wordpress hosting system with a few users (by giving a few licenses away for free) on a cloud VPS. (1-2 days)
5. Verify that the system is working correctly and fix any bugs that may be present.
6. Release the Wordpress hosting system to the public.
7. Finalise the Wordpress hosting system and release the scripts to allow anyone to host their own Wordpress server. (This script will take in a Discord Bot token and set everything up for you on a new linux VPS) (~4 hrs)
8. Order a raspberry pi clone for self hosting to lower costs. (4 wks. not a priority for the project)


## Estimated Cost
The cheapest servers I can find (let me know if you know of a cheaper one):

Linode Nanode 1 GB - $5 USD/month (~$7.70 AUD)
> 1 CPU Core  
1 GB RAM  
25 GB Storage  
1 TB Transfer  
4 Sites @ $15 USD/yr (~$23 AUD)

OVH VPS 1 - $5.75 AUD/month
> 1 vCore  
2 GB RAM  
20 GB SSD SATA  
4 Sites @ $17.25 AUD/yr

OVH VPS 2 (VLE-2) - $196.25 AUD/yr (yearly payment has a big discount)
> 2 vCores  
2 GB RAM  
20 GB SSD NVMe  
50 GB additional storage  
10 sites @ $20 AUD/yr



---

Alternatively, I could buy a server to host at home. I would probably grab a raspberry pi clone for around $100.
It would need an SSD for storage. Either:
- $40 for a M.2 to USB adapter to use with a spare SSD I have lying around
- $100 for an dedicated external SSD.

> 2 GB Ram  
4 CPU Cores 1.5 GHz  
1 TB SSD Storage  
10 sites @ $10 AUD/yr (pays off after ~2 years)

Downside of this is the connection would be slower than a cloud VPS, but it would be cheaper in the long run.


## POC
I have already created a script to install Wordpress on a linux server.
Here is a rough version of the system. It will be improved to allow easy deployment of additional workers and to allow easy scaling of the system.

https://cloud.woodburn.au/s/wp-poc
