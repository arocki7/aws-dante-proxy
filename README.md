# On-Demand SOCKS5 Proxy in AWS

This Ansible repository is to deploy a Dante SOCKS5 proxy in AWS for VPN purposes.

## Purpose of this playbook

Using this playbook,

- you can deploy and configure dante SOCKS proxy in minutes.
- You can choose which country you want the proxy to be in (depends on AWS regions).
- This will allow to visit certain country-based websites.
- You can use this as private VPN with the help of softwares like proxifier.

## How to deploy

- Edit variables depends on your need.
- Make sure that AWS credentials are configured right to deploy EC2 instances.  
- Run the playbook `ansible-playbook deploy.yml`

## How to decommission

Following playbook will just remove the EC2 instance and leave the rest as it is.  

`ansible-playbook decommission.yml`