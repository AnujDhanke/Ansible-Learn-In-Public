# 📚 Ansible Learn-In-Public Journey

Welcome to my **Ansible Learn-In-Public** repository!

This repository contains my daily notes, hands-on exercises, and projects while learning Ansible as part of my DevOps journey. Every day I document what I learned, the problems I faced, how I solved them, and practical examples.

---

## 🎯 Goal

- Learn Ansible from fundamentals to advanced concepts.
- Build production-style automation playbooks.
- Automate Linux server administration.
- Integrate Ansible with AWS.
- Develop reusable and scalable Infrastructure as Code (IaC) practices.

---

# 📅 Daily Progress

| Day | Topic | Status |
|------|-----------------------------------------------|:------:|
| Day 01 | Introduction, Inventory & Ping Module | ✅ |
| Day 02 | Ad-hoc Commands & First Playbook | ✅ |
| Day 03 | Modules Deep Dive & Ansible Configuration | ✅ |
| Day 04 | Variables, group_vars, host_vars & Facts | ✅ |
| Day 05 | Conditionals, Loops & Template Module | ✅ |
| Day 06 | Handlers, Roles & Ansible Galaxy | ✅ |
| Day 07 | Ansible for AWS (IAM, boto3, ec2_key & ec2_instance) | ✅ |

---

# 📂 Repository Structure

```
.
├── Day-01
├── Day-02
├── Day-03
├── Day-04
├── Day-05
├── Day-06
├── Day-07
└── README.md
```

---

# 📖 Daily Topics

## ✅ Day 01 — Introduction to Ansible

- What is Ansible
- Agentless Architecture
- Inventory
- Inventory Groups
- Children Groups
- Variables in Inventory
- Ping Module
- SSH Connectivity

---

## ✅ Day 02 — Ad-hoc Commands & First Playbook

- Ad-hoc Commands
- Common Modules
- Idempotency
- YAML Basics
- Writing First Playbook
- Playbook Validation
- Dry Run
- Verbosity
- PLAY RECAP

---

## ✅ Day 03 — Modules & Configuration

- Built-in vs Community Modules
- ansible.cfg
- Ansible Search Path
- Module Documentation
- ansible-doc
- ansible-galaxy
- Module Dependencies
- Python Interpreter Discovery

---

## ✅ Day 04 — Variables

- Playbook Variables
- Inventory Variables
- group_vars
- host_vars
- Variable Precedence
- Debug Module
- Register Variables
- Setup Module
- Facts
- Fact Variables

---

## ✅ Day 05 — Conditionals, Loops & Templates

- when Condition
- Decision Making
- Loop Keyword
- item Variable
- Loop with Dictionaries
- Template Module
- Jinja2 Templates
- Dynamic Configuration Files

---

## ✅ Day 06 — Handlers & Roles

- Handlers
- notify
- Role Directory Structure
- tasks/
- handlers/
- vars/
- defaults/
- templates/
- files/
- meta/
- Ansible Galaxy
- Variable Priority inside Roles

---

## ✅ Day 07 — Ansible for AWS

- How Ansible manages AWS resources
- API-based automation using boto3
- IAM User & Access Keys
- AWS Authentication using Environment Variables
- Installing boto3 and amazon.aws Collection
- AWS Playbook Structure
- localhost-based AWS Playbooks
- Creating EC2 Key Pairs using `amazon.aws.ec2_key`
- Using `register` to capture module output
- Saving private keys securely using `copy`
- Launching EC2 Instances with `amazon.aws.ec2_instance`
- Using `exact_count` for idempotency
- Managing AWS Regions
- Common AWS module errors and troubleshooting
- Ansible vs Terraform for AWS provisioning

---

# 🛠 Tech Stack

- Ansible
- Linux
- AWS EC2
- AWS IAM
- Python (boto3)
- Git
- GitHub

---

# 📌 Learning Approach

Every day includes:

- 📖 Well-structured notes
- 💻 Hands-on labs
- 🧪 Practical playbooks
- 🐞 Errors encountered
- ✅ Troubleshooting steps
- 🚀 GitHub updates
- 💼 LinkedIn Learn-in-Public posts

---

## ⭐ If you find this repository useful, feel free to star it!