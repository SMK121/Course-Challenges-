# Course-Challenges-


# 🚀 My Biggest Challenges on the Course

This document highlights the main technical challenges I faced during the course, how I approached solving them, and the key lessons I learned.

---

# 🖥️ Challenge 1 - Understanding AWS Instances, AMIs and Resource Management

**Status:** ✅ Solved

## 🔍 The Challenge

One of the challenges I faced was understanding the difference between **AWS EC2 Instances** and **AMI (Amazon Machine Image) images**, especially when managing and cleaning up resources.

Initially, I found it confusing to understand which resources were active and which were templates used for future deployments.

The main difference was understanding:

- 🖥️ **EC2 Instance** → A running virtual machine used to host applications and services
- 📦 **AMI** → A reusable template used to create new EC2 instances

During clean-up tasks, I was unsure whether AMIs should be deleted alongside instances because they appeared connected.

---

## 🛠️ How I Solved It

- Learned the AWS resource lifecycle:

```
Create EC2 Instance
        ↓
Configure Environment
        ↓
Create AMI
        ↓
Launch New Instances From AMI
```

- Checked resource details before deleting anything
- Used clearer naming conventions to identify resources
- Applied feedback from trainers and teammates during AWS resource management tasks

---

## 💡 What I Learned

I learned that effective cloud management requires understanding the purpose of each resource before making changes.

Not every resource associated with an instance should be removed. Some resources, such as AMIs, are designed for **reuse, backups, and faster deployment**.

---

<br>

# 🌐 Challenge 2 - Understanding Security Groups and Network Access

**Status:** ✅ Solved

## 🔍 The Challenge

Understanding how AWS Security Groups control communication between resources was challenging at first.

When connecting an **Application VM** to a **Database VM**, several components needed to be configured correctly:

- 🔒 Security Group rules
- 🔌 Required ports
- 🌍 Private and public IP addresses
- 🗄️ Database access permissions

For example:

- The application needed access to MongoDB through **port 27017**
- The database should not be publicly exposed
- Only required traffic should be allowed

---

## 🛠️ How I Solved It

- Tested communication between VMs step-by-step
- Reviewed inbound and outbound Security Group rules
- Learned the purpose of each port being opened
- Used troubleshooting commands to identify connection issues
- Followed a structured approach instead of changing multiple settings at once

---

## 💡 What I Learned

I learned that cloud networking is not just about making connections work, but understanding **why access is required and how to keep resources secure**.

Security Groups are an important part of controlling communication between cloud resources.

---

<br>

# 💻 Challenge 3 - Learning Linux, Git Bash and AWS VM Commands

**Status:** 🔄 Ongoing, but improved

## 🔍 The Challenge

A major challenge was learning the number of commands used across different environments and understanding when each command should be used.

During the course, I worked across multiple environments:

- 🖥️ Local machine using Git Bash
- 🐧 Ubuntu Linux AWS Virtual Machines
- ☁️ AWS management tools
- ⚙️ Application and service management commands

The challenge was not only remembering commands, but understanding:

- Where the command should be executed
- What the command does
- Why it is needed

---

## 🛠️ How I Solved It

Created personal command notes grouped by purpose:

```
📁 File Management
🔐 Permissions
🌐 Networking
🔄 Git Commands
☁️ AWS Commands
⚙️ Service Management
```

Practised commonly used commands:

```bash
pwd        # Check current directory
ls         # List files and folders
cd         # Change directory
systemctl  # Manage Linux services
ssh        # Connect to remote machines
```

Other improvements:

- Checked my current environment before running commands
- Confirmed whether I was working locally or connected to a VM
- Practised commands through real deployment tasks instead of only memorising them

---

## 💡 What I Learned

I learned that becoming comfortable with the command line comes from understanding the purpose behind commands rather than simply memorising syntax.

Through repeated practice, I became more confident identifying:

- ✅ Which command to use
- ✅ Where to run it
- ✅ What outcome to expect

---

# 🎯 Overall Reflection

These challenges helped improve my confidence working with:

- ☁️ Cloud infrastructure
- 🖥️ AWS services
- 🐧 Linux environments
- 🌐 Networking concepts
- ⚙️ Application deployment

The biggest improvement has been moving from simply following instructions to understanding **why each command, configuration, and resource is required**.

This has helped me become more independent when troubleshooting issues and deploying cloud-based applications.

