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
- Tested playbooks using Dry Run (`-C`)
- Used verbosity flags (`-v`, `-vv`, `-vvv`) for debugging
- Analyzed the `PLAY RECAP` output

---

### ✅ Day 03 – Modules Deep Dive & Ansible Configuration

#### Topics Covered
- Working with Ansible Modules
- Module Workflow
- Built-in vs Community Modules
- `ansible-galaxy`
- Module Requirements
- Python Dependencies
- MySQL Community Modules
- Advanced `copy` Module
- `ansible.cfg`
- Configuration Priority
- Ansible Configuration Sections

#### Hands-on Practice
- Learned how to search and use Ansible modules from the official documentation
- Installed community collections using `ansible-galaxy`
- Understood how community modules differ from built-in modules
- Learned how module dependencies work on target machines
- Explored MySQL/MariaDB community modules
- Configured a project-level `ansible.cfg`
- Set default inventory and privilege escalation options
- Learned how to simplify commands using `ansible.cfg`
- Explored logging and parallel execution settings

#### Key Learnings
- Reading the official module documentation is an essential DevOps skill.
- Community collections are installed on the Control Node using `ansible-galaxy`.
- Some modules require additional Python packages on the target machine.
- Project-level `ansible.cfg` should always be committed to Git for consistent team environments.

---

## 🛠️ Lab Environment

| Component | Details |
|-----------|---------|
| Control Node | Ubuntu EC2 |
| Managed Nodes | 3 × CentOS EC2 |
| Automation Tool | Ansible |
| Cloud Platform | AWS EC2 |



## 📸 Screenshots

The `screenshots/` directory contains images of:
- Lab setup
- Inventory configuration
- Ad-hoc command execution
- Playbook execution
- Module practice
- Configuration examples
- Terminal outputs

---

## 📝 Notes

The `notes/` directory contains detailed notes for each day's learning, including concepts, commands, examples, troubleshooting, and hands-on practice.

---

## 🎯 Goal

This repository is part of my **Learn in Public** journey, where I document my daily progress in learning Ansible through practical implementation and continuous practice.

Upcoming topics include:

- Variables
- Handlers
- Loops
- Conditionals
- Templates
- Roles
- Ansible Vault
- Ansible Galaxy
- Dynamic Inventory
- Real-world Automation Projects

---

⭐ Thanks for visiting! Feel free to explore the repository and follow along with my Ansible learning journey.