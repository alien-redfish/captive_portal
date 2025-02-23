# Captive Portal - Ansible

Ansible playbook to install nodogsplash captive portal on a fresh raspbian install.

## Description

Use this playbook to install a captive portal on a raspberry pi, this will NOT install any new pages in the /etc/nodogsplash/htdocs directory. It will serve the nodogsplash page.

## Getting Started

### Usage

Install ansible on your host system, place the SSH keys from the host system onto the raspberry pi/pi's that you wish to install the captive portal.

Alter the all.yaml file in group_vars to suit your needs.

Change the hosts.yaml to the IP address/s that you wish to install this on. Hostnames can also be put in here, however Raspbian as default uses the hostname raspberrypi.local. If instlling to multiple Pi's that share the same hostname then please use IP addresses.

To run:

* ansible-playbook -i hosts.yaml playbook.yaml -K

The raspberry pi MUST be connected to the internet as it will pull the latest nodogsplash code from its github repository.

## Authors

Contributors names and contact info

ex. alien-redfish  
ex. alien-redfish@protonmail.com