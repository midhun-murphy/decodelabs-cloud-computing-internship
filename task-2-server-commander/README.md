# Server Commander - DecodeLabs Project 2

## Project Overview

Provisioned and configured an AWS EC2 Ubuntu server,
secured SSH access, installed Nginx, and hosted a
custom web application.

---

## Architecture

User Browser
      |
      v
Security Group
      |
      v
AWS EC2 Instance
      |
      v
Ubuntu Linux
      |
      v
Nginx Web Server
      |
      v
Custom HTML Website

---

## Technologies Used

- AWS EC2
- Ubuntu Linux
- SSH
- Nginx
- Security Groups

---

## Commands Used

### Update Server

sudo apt update

### Install Nginx

sudo apt install nginx -y

### Start Nginx

sudo systemctl start nginx

### Enable Nginx

sudo systemctl enable nginx

---

## Outcome

Successfully deployed a static website on AWS EC2
using Nginx and verified accessibility through a
public IP address.
