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
- Fixed Host Key Verification issues
- Resolved inventory permission errors using `chmod 400`

---

## ✅ Day 02 – Ad-hoc Commands & My First Playbook

### Topics Covered
- Ad-hoc Commands
- Core Ansible Modules
- Privilege Escalation (`--become`)
- Idempotency
- YAML Basics
- Playbook Structure
- Gathering Facts
- Playbook Execution
- Debugging Playbooks
- PLAY RECAP

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

### Challenges Solved
- Fixed privilege escalation issues using `--become`
- Corrected YAML indentation mistakes

---

## ✅ Day 03 – Modules Deep Dive & Ansible Configuration

### Topics Covered
- Built-in vs Community Modules
- Module Documentation
- `ansible-galaxy`
- Community Collections
- Python Dependencies
- MySQL Modules
- Advanced `copy` Module
- `ansible.cfg`
- Configuration Priority
- Logging & Parallelism

### Hands-on Practice
- Installed community collections using `ansible-galaxy`
- Explored official module documentation
- Configured a project-level `ansible.cfg`
- Set default inventory and privilege escalation
- Explored MySQL community modules

### Challenges Solved
- Installed missing Python dependencies
- Understood interpreter discovery warnings
- Learned how to resolve module deprecation warnings

---

## ✅ Day 04 – Variables, group_vars, host_vars & Fact Variables

### Topics Covered
- Variables
- Variable Syntax
- `group_vars`
- `host_vars`
- `vars_files`
- Variable Precedence
- Variable Types
- Command Line Variables (`-e`)
- `debug`
- `register`
- Fact Variables
- `setup` Module

### Hands-on Practice
- Created reusable variables
- Organized variables using `group_vars` and `host_vars`
- Printed variables using `debug`
- Stored task outputs using `register`
- Retrieved system information using the `setup` module
- Explored OS, CPU, Memory, Hostname and Network facts

### Challenges Solved
- Fixed variable syntax mistakes
- Understood variable precedence
- Learned when Fact Variables become unavailable

---

## ✅ Day 05 – Conditionals, Loops & Template Module

### Topics Covered
- Decision Making using `when`
- Loops using the `loop` keyword
- The `item` variable
- Installing multiple packages
- Creating multiple users
- Looping over Variables
- Looping through Dictionaries
- Jinja2 Templates
- Template Module
- Dynamic Configuration Files
- Difference between `copy` and `template`

### Hands-on Practice
- Executed OS-specific tasks using `when`
- Installed multiple packages using loops
- Created users with loops
- Used variables inside loops
- Printed loop values using `debug`
- Generated dynamic configuration files using the `template` module
- Added a custom MOTD banner
- Restarted services after configuration changes

### Challenges Solved
- Fixed loop execution issues caused by incorrect `item` usage
- Corrected NTP template deployment errors
- Understood when to use `copy` vs `template`
- Improved playbook readability using loops

---

## ✅ Day 06 – Handlers, Roles & Ansible Galaxy

### Topics Covered
- Handlers
- `notify` Keyword
- Handler Execution Flow
- Multiple Handlers
- Ansible Roles
- Standard Role Directory Structure
- `tasks/main.yml`
- `handlers/main.yml`
- `defaults/main.yml`
- `vars/main.yml`
- Templates & Files inside Roles
- Variable Priority in Roles
- Ansible Galaxy
- Community Roles

### Hands-on Practice
- Created Handlers using the `notify` keyword
- Restarted services only when configuration files changed
- Built reusable Roles using `ansible-galaxy init`
- Organized tasks, handlers, templates, files, defaults and vars inside a Role
- Converted an existing provisioning playbook into a reusable Role
- Installed and explored community roles from Ansible Galaxy
- Learned how Role variables can be overridden

### Challenges Solved
- Understood why handlers execute only when a task reports `changed`
- Learned the exact relationship between `notify` and handler names
- Organized large playbooks into modular Role structures
- Understood the difference between `defaults` and `vars` inside Roles

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
├── roles/
├── notes/
│   ├── Day-01.md
│   ├── Day-02.md
│   ├── Day-03.md
│   ├── Day-04.md
│   ├── Day-05.md
│   └── Day-06.md
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
- Conditional Execution
- Loops
- Template Module
- Handlers
- Roles
- Configuration Examples
- Terminal Outputs

---

# 📝 Notes

The `notes/` directory contains detailed notes for each day's learning, including concepts, commands, examples, troubleshooting, and hands-on practice.

---

# 🎯 Goal

This repository is part of my **Learn in Public** journey, where I document my daily progress in learning Ansible through practical implementation and continuous hands-on practice.

### Upcoming Topics

- Ansible Vault
- Dynamic Inventory
- Tags
- Error Handling
- Real-world Automation Projects
- Ansible + Terraform Integration
- Ansible + Kubernetes Integration

---

⭐ If you're also learning Ansible, feel free to explore this repository and follow along with my daily learning journey.