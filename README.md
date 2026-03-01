## aws-ec2-project
# deploy a simple web applovation on AWS EC2
- This project demonstrates how to deploy a simple web application (such as Jenkins) on an AWS EC2 instance and make it accessible from outside AWS. It includes steps for provisioning resources, configuring the server, and accessing the application via a public URL.
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
- Linux (Amazon Linux / Ubuntu)
- Apache Web Server
- HTML
- SSH

User Browser
|
v
Public Internet
|
v
AWS EC2 Instance
|
v
Apache Web Server
|
v
HTML Web Application


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

### 2. Connect to EC2

```bash
ssh -i "your-key.pem" ec2-user@your-public-ip


---

## Project Architecture
