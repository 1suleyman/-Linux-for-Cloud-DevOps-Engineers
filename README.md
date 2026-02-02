# 🐧 Linux for Cloud & DevOps Engineers

This repository documents a hands-on Linux project focused on how systems actually behave once they’re running — and when they don’t behave as expected.

Rather than treating Linux as a list of commands to memorise, this project treats it as an environment to reason about:
how users are created, how permissions interact, how storage survives reboots, how automation behaves at boot time, and how to verify that changes really took effect.

The labs mirror the kind of work that happens on real Linux servers:
making changes safely, validating assumptions, debugging unexpected state, and cleaning up environments you don’t want lingering.

Each lab builds on the previous one and mirrors **real-world DevOps tasks** you’d expect when working with Linux servers in production.

---

## 📚 Project Focus

This project explores core Linux areas that tend to surface once systems are live and under use:

* User and group management, including primary vs supplementary groups
* Permissions, ownership, and access boundaries
* File and directory operations with attention to safety and context
* Text processing and repeatable edits using standard CLI tools
* Boot-time automation and validation
* Linux storage behaviour when integrated with AWS EC2 + EBS
* Auditing, cleanup, and teardown to return systems to a known state

Each lab is documented in its own folder with a concise README covering:

* the setup
* what was observed
* how changes were verified
* and what stood out during the process

---

## 🧪 Lab Structure

This project is intentionally split into **focused labs** to keep learning structured, practical, and portfolio-ready.

### 🔹 Lab 0: Infrastructure Bootstrap (Terraform)

| Lab | Title                    | Link             | Key Skill                                                            |
| --- | ------------------------ | ---------------- | -------------------------------------------------------------------- |
| 0   | Infrastructure Bootstrap | 📂 [Repo](https://github.com/1suleyman/-Lab-0-Infrastructure-Bootstrap-Terraform-/tree/main) | Provisioning EC2 with Terraform, SSH access, tagging, reusable infra |

---

### 🔹 Lab 1: Users, Groups & Permissions

| Lab | Title                     | Link                    | Key Skill                                                                  |
| --- | ------------------------- | ----------------------- | -------------------------------------------------------------------------- |
| 1   | Users & Groups Management | 📂 [Repo](https://github.com/1suleyman/-Linux-Users-Groups-Permissions-Lab-1/tree/main) | Creating users/groups, primary & secondary groups, ownership & permissions |
| 2   | Linux Users/Groups Bootstrap Automation — Part 1 (Code Walkthrough) | 📂 [Repo](https://github.com/1suleyman/-Linux-Users-Groups-Bootstrap-Automation-Lab-user_data.sh-Part-1-Code-Walkthrough-) | Bash scripting fundamentals, user_data.sh logic walkthrough, arrays & loops, exit-code driven logic, stdout/stderr redirection, chpasswd usage, idempotent design |
| 3   | Linux Users/Groups Bootstrap Automation — Part 2 (Testing + Debugging) | 📂 [Repo](https://github.com/1suleyman/-Linux-Lab-1-Bootstrap-Automation-user_data.sh-Part-2-Testing-Debugging-) | Cloud-init debugging, Terraform user_data validation, PATH troubleshooting, env -i reproduction, Bash reserved variables, log-driven debugging, engineering trade-off analysis |

---

### 🔹 Lab 2: Files & Directory Operations

| Lab | Title                 | Link                         | Key Skill                                                          |
| --- | --------------------- | ---------------------------- | ------------------------------------------------------------------ |
| 2   | Linux Files & Directory Operations (User Switching + CLI) | 📂 [Repo](https://github.com/1suleyman/-Linux-Files-Directory-Operations-Lab-2-User-Switching-Real-CLI-Work-/tree/main) | Linux user switching, sudoers.d configuration, privilege escalation, mkdir/touch/mv/rm, relative paths & wildcards, safe deletions, real-world permission troubleshooting |

---

### 🔹 Lab 3: Text Processing & Vi Editor

| Lab | Title                     | Link                       | Key Skill                                                             |
| --- | ------------------------- | -------------------------- | --------------------------------------------------------------------- |
| 3   | Linux Text Processing & VI (Search / Replace) | 📂 [Repo](https://github.com/1suleyman/Linux-Text-Processing-VI-Lab/tree/main) | Linux text processing, sed in-place editing, vi search & replace, user switching best practices, sudo via wheel, safe recursive deletes, output verification |

---

### 🔹 Lab 4: Storage & Filesystems (AWS EBS)

| Lab | Title                  | Link                   | Key Skill                                                     |
| --- | ---------------------- | ---------------------- | ------------------------------------------------------------- |
| 4   | Linux Storage & File Systems Lab (EBS → Mount + Persistence) | 📂 [Repo](https://github.com/1suleyman/Linux-Storage-File-Systems-Lab/tree/main) | EBS attachment, lsblk, mkfs (xfs/ext4), mount, /etc/fstab, UUID, nofail, mount -a |

---

### 🔹 Lab 5: Cleanup, Auditing & Teardown

| Lab | Title              | Link               | Key Skill                                                          |
| --- | ------------------ | ------------------ | ------------------------------------------------------------------ |
| 5   | Linux Cleanup & Teardown Lab (Audit → Remove → Destroy) | 📂 [Repo](https://github.com/1suleyman/Linux-Cleanup-Teardown-Lab/tree/main) | Idempotent cleanup, find + stderr redirection, userdel/groupdel, sed fstab edits, safe unmounting, EBS detach/delete, terraform destroy |

---

## 🧠 Why This Repository Exists

This repository reflects how I approach Linux systems:

* configure carefully
* verify explicitly
* assume less
* clean up properly

It’s a record of learning how Linux behaves in environments where small details tend to matter.

---

## 📌 Final Note

Linux isn’t difficult because the commands are complex.
It’s difficult because it’s easy to assume things worked when they didn’t.

This project is my way of getting comfortable with that gap — and closing it deliberately.
