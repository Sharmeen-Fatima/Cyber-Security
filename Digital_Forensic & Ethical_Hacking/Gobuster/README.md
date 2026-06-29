# Gobuster

## 📌 Overview

Gobuster is a fast and powerful command-line tool written in Go. It is commonly used by cybersecurity professionals and penetration testers to discover hidden files, directories, subdomains, DNS records, virtual hosts, and cloud storage buckets.

Gobuster helps security researchers identify resources that are not directly linked on a website but are still accessible.

> **Note:** This tool should only be used on systems that you own or have explicit permission to test.

---

# 🎯 Why Use Gobuster?

During a penetration test, many websites contain hidden directories or files that are not visible through normal browsing.

Gobuster helps security professionals:

- Discover hidden directories
- Find sensitive files
- Enumerate subdomains
- Detect virtual hosts
- Test cloud storage buckets
- Improve security assessments

It is widely used during the **Information Gathering** and **Enumeration** phases of ethical hacking.

---

# 🔍 What Information Can Gobuster Discover?

Gobuster can help identify:

- Hidden directories
- Hidden web pages
- Backup files
- Configuration files
- Login portals
- Admin panels
- API endpoints
- Development folders
- Test environments
- Subdomains
- Virtual Hosts (VHOST)
- DNS records
- Public cloud storage buckets (depending on the selected mode)

> Gobuster only discovers resources that exist and are accessible. It does **not** exploit vulnerabilities.

---

# ⚙️ How Does Gobuster Work?

Gobuster performs **wordlist-based enumeration**.

The process is simple:

1. The user provides a target URL or domain.
2. A wordlist containing thousands of common names is loaded.
3. Gobuster combines each word with the target.
4. It sends HTTP or DNS requests.
5. It analyzes the server responses.
6. Valid results are displayed to the user.

Example:

Target:

https://example.com

Wordlist:

```
admin
login
backup
images
test
```

Gobuster checks:

```
https://example.com/admin
https://example.com/login
https://example.com/backup
https://example.com/images
https://example.com/test
```

If a resource exists, Gobuster reports it.

---

# 🚀 Gobuster Modes

Gobuster supports multiple modes:

- Directory Enumeration (dir)
- DNS Enumeration (dns)
- Virtual Host Enumeration (vhost)
- S3 Bucket Enumeration (s3)
- GCS Bucket Enumeration (gcs)
- Fuzzing (fuzz)

Each mode is designed for a different type of security assessment.

---

# 💡 Common Use Cases

Gobuster is commonly used for:

- Web Application Security Testing
- Penetration Testing
- Bug Bounty Hunting
- Red Team Assessments
- Security Audits
- Capture The Flag (CTF) Practice
- Cybersecurity Learning Labs

---

# 📚 Key Features

- Fast and lightweight
- Multi-threaded scanning
- Easy to use
- Open-source
- Written in Go
- Supports multiple enumeration modes
- Works on Linux, Windows, and macOS

---

# 🛡️ Ethical Use

Gobuster is intended for **authorized security testing only**.

Always ensure you have permission before scanning any website, server, or network. Unauthorized scanning may violate laws or organizational policies.

---

# 📖 Learning Outcome

After learning Gobuster, you will understand:

- What directory enumeration is
- How hidden resources are discovered
- How wordlists are used
- How reconnaissance supports penetration testing
- How to identify exposed web resources during authorized assessments

---

# 📄 License

This repository is created for educational purposes to help students and cybersecurity learners understand how Gobuster works in ethical hacking.
