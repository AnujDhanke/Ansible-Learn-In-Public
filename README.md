# Ansible Learning Journey 🚀

This repository contains my hands-on practice, notes, and screenshots from learning **Ansible** as part of my DevOps journey.

## 📚 Topics Covered

- Introduction to Ansible
- Ansible Architecture
- Inventory File
- Inventory Groups
- Child Groups (`children`)
- Group Variables (`vars`)
- Ansible Ping Module
- SSH Connectivity
- Host Key Verification
- Inventory File Permission (`chmod 400`)

## 🛠️ Lab Setup

- **Control Node**
  - Ubuntu EC2 Instance

- **Managed Nodes**
  - CentOS EC2 Instance 1
  - CentOS EC2 Instance 2
  - CentOS EC2 Instance 3

The Ubuntu EC2 instance acts as the Ansible Control Node and manages all three CentOS instances.

## 💻 What I Practiced

- Created and configured an inventory file
- Organized hosts using groups
- Used `children` and `vars` in the inventory
- Verified connectivity using the `ping` module
- Fixed common Ansible errors:
  - Host key verification failed
  - Inventory file permission issue (`chmod 400`)

## 📸 Screenshots

Screenshots of the lab setup and command outputs are available in the `screenshots/` directory.

## 📝 Notes

Detailed notes for each topic are available in the `notes/` directory.

## 📂 Repository Structure

```
.
├── inventory/
├── notes/
├── screenshots/
├── ansible.cfg
└── README.md
```

## 🎯 Goal

This repository is part of my **Learn in Public** journey, where I document my daily DevOps learning, hands-on practice, and progress with Ansible.

---

⭐ Feel free to explore the notes and follow along with my learning journey!