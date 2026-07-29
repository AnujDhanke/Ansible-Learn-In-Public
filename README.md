# Ansible Learning Journey 🚀

This repository documents my hands-on learning of **Ansible** as part of my DevOps journey. It contains daily notes, practical exercises, screenshots, and playbooks created while following my DevOps course.

---

# 📚 Learning Progress

## ✅ Day 01 – Introduction to Ansible & Inventory

### Topics Covered
- Introduction to Ansible
- Ansible Architecture
- Inventory File
- Inventory Groups
- Child Groups (`children`)
- Group Variables (`vars`)
- Ansible Ping Module

### Hands-on Practice
- Configured an Ubuntu EC2 instance as the Ansible Control Node
- Connected and managed three CentOS EC2 instances
- Created an Inventory file
- Organized hosts using groups, children, and vars
- Verified connectivity using the `ping` module

### Challenges Solved
- Host Key Verification error
- Inventory permission issue using `chmod 400`

---

## ✅ Day 02 – Ad-hoc Commands & My First Playbook

### Topics Covered
- Ad-hoc Commands
- Core Ansible Modules
- Privilege Escalation (`--become`)
- Idempotency
- Playbook Structure
- YAML Indentation
- Gathering Facts
- Running Playbooks
- Debugging Playbooks

### Modules Learned
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

### Hands-on Practice
- Executed Ad-hoc Commands
- Installed packages using the `yum` module
- Managed services using the `service` module
- Practiced Idempotency
- Wrote and executed my first Playbook
- Validated playbooks using `--syntax-check`
- Tested playbooks using Dry Run (`-C`)
- Used verbosity flags (`-v`, `-vv`, `-vvv`)
- Analyzed `PLAY RECAP`

### Challenges Solved
- Fixed privilege escalation issues using `--become`
- Corrected YAML indentation mistakes

---

## ✅ Day 03 – Modules Deep Dive & Ansible Configuration

### Topics Covered
- Working with Ansible Modules
- Built-in vs Community Modules
- `ansible-galaxy`
- Module Requirements
- Python Dependencies
- MySQL Community Modules
- Advanced `copy` Module
- `ansible.cfg`
- Configuration Priority
- Ansible Configuration Sections

### Hands-on Practice
- Installed community collections using `ansible-galaxy`
- Explored official module documentation
- Learned module dependencies
- Configured project-level `ansible.cfg`
- Configured inventory, logging, and privilege escalation

### Challenges Solved
- Installed missing Python dependencies required by MySQL modules
- Understood Python Interpreter Discovery warnings
- Learned how to resolve deprecation warnings

---

## ✅ Day 04 – Variables, group_vars, host_vars & Fact Variables

### Topics Covered
- Custom Variables
- Variable Syntax
- `vars`
- `group_vars`
- `host_vars`
- `vars_files`
- Variable Precedence
- Command Line Variables (`-e`)
- Variable Types
- `debug` Module
- `register`
- Fact Variables
- `setup` Module
- Gathering Facts

### Hands-on Practice
- Created reusable variables
- Organized variables using `group_vars` and `host_vars`
- Used the `debug` module
- Stored task outputs using `register`
- Retrieved system facts using the `setup` module
- Explored OS, CPU, Memory, Hostname and Network facts

### Challenges Solved
- Fixed variable syntax issues
- Understood variable precedence
- Learned when Fact Variables are unavailable (`gather_facts: false`)

---

## ✅ Day 05 – Conditionals, Loops & Template Module

### Topics Covered
- Decision Making using `when`
- Loops using the `loop` keyword
- The `item` variable
- Installing multiple packages with loops
- Creating multiple users with loops
- Looping over Variables
- Looping through Dictionaries
- Using `debug` with loops
- Jinja2 Templates
- Template Module
- Dynamic Configuration Files
- Difference between `copy` and `template` modules

### Hands-on Practice
- Executed tasks conditionally using `when`
- Installed multiple packages using a single loop
- Created multiple users using loops
- Used variables inside loops
- Printed loop values using `debug`
- Iterated through dictionaries using `item.name`
- Generated dynamic configuration files using the `template` module
- Compared `copy` vs `template` modules

### Challenges Solved
- Fixed undefined variable errors caused by using `item` outside loops
- Corrected YAML indentation for loop blocks
- Learned the correct use cases for `copy` and `template`
- Practiced writing accurate conditional statements

---

# 🛠️ Lab Environment

| Component | Details |
|-----------|---------|
| Control Node | Ubuntu EC2 |
| Managed Nodes | 3 × CentOS EC2 |
| Cloud Platform | AWS EC2 |
| Automation Tool | Ansible |

---

# 📂 Repository Structure

```text
.
├── inventory/
├── playbooks/
├── group_vars/
├── host_vars/
├── templates/
├── notes/
│   ├── Day-01.md
│   ├── Day-02.md
│   ├── Day-03.md
│   ├── Day-04.md
│   └── Day-05.md
├── screenshots/
├── ansible.cfg
└── README.md
```

---

# 📸 Screenshots

The `screenshots/` directory contains images of:

- Lab Setup
- Inventory Configuration
- Ad-hoc Commands
- Playbook Execution
- Variables Practice
- Loop Examples
- Template Module Examples
- Configuration Examples
- Terminal Outputs

---

# 📝 Notes

The `notes/` directory contains detailed notes for each day's learning, including concepts, examples, commands, troubleshooting, and hands-on practice.

---

# 🎯 Goal

This repository is part of my **Learn in Public** journey, where I document my daily progress in learning Ansible through practical implementation and continuous hands-on practice.

Upcoming topics include:

- Roles
- Role Directory Structure
- Ansible Galaxy Roles
- Ansible Vault
- Dynamic Inventory
- Tags
- Error Handling
- Real-world Automation Projects

---

⭐ If you're also learning Ansible, feel free to explore this repository and follow along with my daily learning journey.