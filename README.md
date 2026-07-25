# Ansible Learning Journey 🚀

This repository documents my hands-on learning of **Ansible** as part of my DevOps journey. It contains daily notes, practical exercises, screenshots, and playbooks created while following my DevOps course.

---

## 📚 Learning Progress

### ✅ Day 01 – Introduction to Ansible & Inventory

#### Topics Covered
- Introduction to Ansible
- Ansible Architecture
- Inventory File
- Inventory Groups
- Child Groups (`children`)
- Group Variables (`vars`)
- Ansible Ping Module

#### Hands-on Practice
- Configured an Ubuntu EC2 instance as the Ansible Control Node
- Connected and managed three CentOS EC2 instances
- Created an Inventory file
- Organized hosts using groups, children, and vars
- Verified connectivity using the `ping` module
- Resolved:
  - Host Key Verification error
  - Inventory permission issue using `chmod 400`

---

### ✅ Day 02 – Ad-hoc Commands & My First Playbook

#### Topics Covered
- Ad-hoc Commands
- Core Ansible Modules
- Privilege Escalation (`--become`)
- Idempotency
- Playbook Structure
- YAML Indentation
- Gathering Facts
- Running Playbooks
- Debugging Playbooks

#### Modules Learned
- yum / apt
- service
- copy
- file
- command
- shell
- get_url
- unarchive
- ping
- setup

#### Hands-on Practice
- Executed multiple Ad-hoc Commands
- Installed packages using the `yum` module
- Managed services using the `service` module
- Practiced Idempotency
- Wrote and executed my first Ansible Playbook
- Validated playbooks using `--syntax-check`
- Used dry-run mode (`-C`)
- Debugged playbooks using verbosity flags (`-v`, `-vv`, `-vvv`)
- Analyzed the `PLAY RECAP` output

---

## 🛠️ Lab Environment

| Component | Details |
|-----------|---------|
| Control Node | Ubuntu EC2 |
| Managed Nodes | 3 × CentOS EC2 |
| Automation Tool | Ansible |
| Cloud Platform | AWS EC2 |

---

## 📂 Repository Structure

```
.
├── playbooks/
├── inventory/
├── notes/
│   ├── Day-01.md
│   └── Day-02.md
├── screenshots/
├── README.md
```

---

## 📸 Screenshots

The `screenshots/` directory contains images of:
- Lab setup
- Inventory configuration
- Ad-hoc command execution
- Playbook execution
- Terminal outputs

---

## 📝 Notes

The `notes/` directory contains detailed notes for each day's learning, including concepts, commands, examples, and troubleshooting steps.

---

## 🎯 Goal

This repository is part of my **Learn in Public** journey, where I document my daily progress in learning Ansible through practical implementation and continuous practice.

More daily updates will be added as I continue exploring:
- Variables
- Conditionals
- Loops
- Handlers
- Templates
- Roles
- Ansible Vault
- Ansible Galaxy
- Real-world automation projects

---

⭐ Thanks for visiting! Feel free to explore the repository and follow along with my Ansible learning journey.