# 🧱 AWS Mini Project: Load Balanced Auto-Healing Apache App using EC2 + ELB + ASG

👤 **Author**: Aryan Kaushik  
📅 **Date**: 2025-06-25

---

## 🎯 Objective

This mini project demonstrates how to deploy a **scalable and fault-tolerant Apache web application** using:

- EC2 (Ubuntu) + Apache via User Data
- Application Load Balancer (ALB)
- Auto Scaling Group (ASG)
- With full clean-up and screenshots

---

## 🧰 Tools & AWS Services Used

- EC2 (Ubuntu 22.04 or Amazon Linux 2023)
- User Data script (for Apache install)
- Application Load Balancer (ALB)
- Target Group
- Launch Template
- Auto Scaling Group (ASG)
- Security Groups
- AWS Management Console

---

## 📁 Files Included

- 📄 [`AWS_ELB_ASG_MiniProject_Aryan.pdf`](AWS_ELB_ASG_MiniProject_Aryan.pdf)  
  ➤ Complete step-by-step guide with screenshots and clean-up process

---

## 📌 Highlights

✅ Apache installed via EC2 User Data  
✅ Load Balancer distributes traffic across instances  
✅ Auto Scaling Group ensures auto-healing  
✅ DNS of ALB always serves the app  
✅ Clean-up done at the end to avoid AWS charges  
✅ Screenshots with figure numbers added in PDF

---

## 🧱 Project Architecture Overview

The project follows this AWS infrastructure flow:

1. **EC2 Instance (Ubuntu)**  
   ➤ Apache web server installed using User Data  
   ➤ Unique hostname shows which instance served the request

2. **Application Load Balancer (ALB)**  
   ➤ Balances HTTP traffic between multiple EC2 instances  
   ➤ DNS remains constant even if backend instances change

3. **Target Group**  
   ➤ Attached to ALB and monitored for health checks  
   ➤ Automatically reflects healthy/unhealthy instances

4. **Launch Template**  
   ➤ Stores AMI, instance type, SG, and User Data  
   ➤ Used by Auto Scaling Group

5. **Auto Scaling Group (ASG)**  
   ➤ Launches EC2 instances from Launch Template  
   ➤ Maintains desired capacity  
   ➤ Automatically replaces terminated instances (Auto Healing)

📦 ➝ 🎯 ➝ 🌀 ➝ 🚀  
EC2 ➝ Target Group ➝ ALB ➝ ASG

---

## 🧹 Clean-Up (To Avoid AWS Billing)

To avoid charges, delete the following resources **in order**:

1. ✅ Delete Auto Scaling Group (ASG)
2. ✅ Delete Launch Template
3. ✅ Delete Load Balancer (ALB)
4. ✅ Delete Target Group
5. ✅ Terminate EC2 Instances

---

## 🚀 Outcome

- ✅ Web app runs with Apache on EC2  
- ✅ Load balanced across AZs with ALB  
- ✅ Auto Healing via ASG tested  
- ✅ DNS stays stable  
- ✅ Billing remains under control  
- ✅ Project is job/internship


