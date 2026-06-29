# Gobuster Cheat Sheet

## 📌 Quick Overview

**Gobuster** is a fast command-line enumeration tool used during authorized security assessments to discover hidden directories, files, subdomains, virtual hosts, and cloud storage buckets.

---

# Basic Syntax

```bash
gobuster [mode] [options]
```

---

# Available Modes

| Mode  | Description                             |
| ----- | --------------------------------------- |
| dir   | Directory and file enumeration          |
| dns   | DNS subdomain enumeration               |
| vhost | Virtual host enumeration                |
| fuzz  | URL fuzzing                             |
| s3    | Amazon S3 bucket enumeration            |
| gcs   | Google Cloud Storage bucket enumeration |

---

# Common Options

| Option         | Purpose                       |
| -------------- | ----------------------------- |
| -u             | Target URL                    |
| -d             | Target domain (DNS mode)      |
| -w             | Wordlist                      |
| -t             | Number of threads             |
| -o             | Save output                   |
| -x             | File extensions               |
| -k             | Ignore SSL certificate errors |
| -H             | Custom HTTP header            |
| -c             | Cookie                        |
| --timeout      | Request timeout               |
| --delay        | Delay between requests        |
| --random-agent | Random User-Agent             |

---

# Quick Command Examples

### Directory Enumeration

```bash
gobuster dir -u https://example.com -w wordlist.txt
```

---

### DNS Enumeration

```bash
gobuster dns -d example.com -w subdomains.txt
```

---

### Virtual Host Enumeration

```bash
gobuster vhost -u https://example.com -w wordlist.txt
```

---

### Fuzzing

```bash
gobuster fuzz -u https://example.com/FUZZ -w wordlist.txt
```

---

### Save Output

```bash
gobuster dir -u https://example.com -w wordlist.txt -o results.txt
```

---

### Multiple File Extensions

```bash
gobuster dir -u https://example.com -w wordlist.txt -x php,html,txt
```

---

### Increase Threads

```bash
gobuster dir -u https://example.com -w wordlist.txt -t 50
```

---

### Ignore SSL Errors

```bash
gobuster dir -u https://example.com -w wordlist.txt -k
```

---

### Display Help

```bash
gobuster --help
```

---

### Check Version

```bash
gobuster version
```

---

# Typical Workflow

1. Install Gobuster
2. Select the appropriate mode
3. Choose a suitable wordlist
4. Run the scan
5. Review the results
6. Save findings for documentation

---

# Commonly Discovered Resources

* Admin panels
* Login pages
* Hidden directories
* Backup files
* Configuration files
* API endpoints
* Development folders
* Test environments
* Public subdomains
* Virtual hosts

---

# Best Practices

* Test only authorized targets.
* Use an appropriate wordlist.
* Save scan results.
* Adjust thread count responsibly.
* Verify findings before reporting them.

---

# Common Errors

| Error              | Possible Cause             |
| ------------------ | -------------------------- |
| Command not found  | Gobuster not installed     |
| No such file       | Incorrect wordlist path    |
| Permission denied  | Insufficient permissions   |
| Connection refused | Target unavailable         |
| SSL error          | Untrusted certificate      |
| Timeout            | Slow or unreachable server |

---

# Learning Path

* Learn Gobuster installation.
* Understand enumeration concepts.
* Practice in authorized labs.
* Explore different modes.
* Interpret scan results responsibly.

---

# Quick Reminder

Gobuster is an **enumeration tool**, not an exploitation tool. Its purpose is to help identify accessible resources during authorized penetration testing and security assessments.

---

> 💡 *This README is for educational purposes — designed to help beginners understand the core concepts of Digital_Forensic & Ethical_Hacking clearly and professionally.*

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *29 June 2026*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Digital_Forensic & Ethical_Hacking and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***

