# 🐧 Linux for Cloud & DevOps Engineers

Welcome to more **Linux learning & practice** 👋
This repository documents a **hands-on Linux project** designed specifically for **Cloud & DevOps Engineers**.

The goal of this project is to **build real Linux confidence**, not just memorize commands — covering user management, permissions, file systems, text processing, and cloud-integrated storage using **AWS EC2 + EBS**.

Each lab builds on the previous one and mirrors **real-world DevOps tasks** you’d expect when working with Linux servers in production.

---

## 📚 Project Overview

This project focuses on **core Linux skills every Cloud/DevOps Engineer must master**, including:

👤 Linux user & group management <br>
🔐 Permissions, ownership, and access control <br>
📁 Directory & file operations (absolute & relative paths) <br>
📝 Text processing with `sed`, `grep`, and `vi` <br>
🧠 Command-line efficiency & safety <br>
☁️ Cloud-integrated Linux storage (AWS EC2 + EBS) <br>
🧹 Cleanup, auditing, and environment teardown

Each lab is documented in its **own folder** with a README containing:

✅ Step-by-step commands
🐛 Troubleshooting notes
💡 Key takeaways

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

## 🧠 Why This Project Matters

This repository demonstrates:

✔️ Practical Linux skills used daily by DevOps engineers <br>
✔️ Safe system administration practices <br>
✔️ Cloud + Linux integration (EC2 & EBS) <br>
✔️ Clean environment teardown & cost awareness <br>
✔️ Terraform + Linux working together

This is **not a toy project** — it mirrors real operational work.

---

## 📌 Final Note

> Linux isn’t about memorizing commands —
> it’s about **thinking clearly under pressure on a server you can’t afford to break**.

This project is my way of building that confidence.
