## aws-ec2-project
# AWS EC2 Simple Web Application Deployment

## Project Overview
This project demonstrates how to deploy a simple static web application on an AWS EC2 instance using the Apache web server. It is a basic DevOps beginner project to understand cloud deployment and server setup.

The application is deployed on a Linux-based EC2 instance and accessed through a public IP address using HTTP.

---

## Objectives
- Launch an EC2 instance on AWS
- Connect to the instance using SSH
- Install Apache web server
- Deploy a simple HTML web page
- Configure Security Groups for web access

---

## Technologies Used
- AWS EC2
- Linux (Amazon Linux)
- Apache Web Server
- HTML
- SSH
## Project Architecture

- User Browser
- |
- v
- Public Internet
- |
- v
- AWS EC2 Instance
- |
- v
- Apache Web Server
- |
- v
- HTML Web Application

---

## Step-by-Step Deployment

### 1. Launch EC2 Instance
- Go to AWS Console
- Launch a new EC2 instance
- Choose Amazon Linux or Ubuntu
- Select instance type (t2.micro)
- Create or select a key pair
- Allow:
  - SSH (Port 22)
  - HTTP (Port 80)

---

<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/9a830895-e1c8-4eef-9af3-729ebaf565fd" />

---

### 2. Connect to EC2
- open powershell on your machine
- ssh -i "your-key.pem" ec2-user@your-public-ip

<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/3f4ccaa2-1188-4d0e-b79e-edde54c0dc29" />

---

## 3. Update Packages
- sudo yum update -y
---

## 4. Install Apache
- sudo yum install httpd -y
- sudo systemctl start httpd
- sudo systemctl status httpd
---

## 5. Deploy Web Application
- cd /var/www/html
- sudo nano index.html
- Example HTML:
- Hello World My First AWS EC2 Web Application

# how to save this html page and exit 

- Press Ctrl + X

- Press Y

- Press Enter
---
## 6. Access Website
Enter the public ip on the chrome see on this image and press enter button 
  <img width="1560" height="823" alt="image" src="https://github.com/user-attachments/assets/1c45099f-3544-4f94-a037-51b0dff0d33f" />

---

# Output
The static web page is successfully deployed and accessible over the internet using the EC2 public IP.

<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/6633d935-c88f-45e3-b7d1-7c8216a38422" />

---

## Learning Outcomes
- Basic cloud deployment

- Linux server configuration

- Web server setup

- AWS networking basics

  ---
  # Author
  ### Anoop kumar
  
