# Gobuster Commands

## 📌 Introduction

Gobuster supports multiple modes for different types of enumeration. Each mode has its own command syntax and purpose.

This document explains the most commonly used Gobuster commands.

> **Important:** Use Gobuster only on systems that you own or have explicit permission to test.

---

# Basic Command Syntax

The general syntax is:

```bash
gobuster [mode] [options]
```

Example:

```bash
gobuster dir -u https://example.com -w wordlist.txt
```

---

# Available Modes

Gobuster supports the following modes:

| Mode | Purpose |
|------|---------|
| dir | Directory and file enumeration |
| dns | Subdomain enumeration |
| vhost | Virtual Host enumeration |
| fuzz | Fuzzing URLs and parameters |
| s3 | Amazon S3 bucket enumeration |
| gcs | Google Cloud Storage bucket enumeration |

---

# Common Options

| Option | Description |
|---------|-------------|
| -u | Target URL or domain |
| -w | Wordlist file |
| -t | Number of threads |
| -o | Save output to a file |
| -x | Search for specific file extensions |
| -k | Skip SSL certificate verification |
| -c | Add cookies |
| -H | Add custom HTTP headers |
| -U | Username (Basic Authentication) |
| -P | Password (Basic Authentication) |
| --timeout | Set request timeout |
| --delay | Delay between requests |
| --random-agent | Use a random User-Agent |

---

# Directory Enumeration (dir)

Purpose:

Find hidden directories and files on a website.

Basic Syntax:

```bash
gobuster dir -u https://example.com -w wordlist.txt
```

Commonly Used Options:

```bash
-x php,html,txt
```

```bash
-t 50
```

```bash
-k
```

---

# DNS Enumeration (dns)

Purpose:

Discover subdomains of a target domain.

Syntax:

```bash
gobuster dns -d example.com -w wordlist.txt
```

Useful Option:

```bash
-i
```

Displays the IP address of discovered subdomains.

---

# Virtual Host Enumeration (vhost)

Purpose:

Find hidden virtual hosts configured on a web server.

Syntax:

```bash
gobuster vhost -u https://example.com -w wordlist.txt
```

---

# Fuzz Mode

Purpose:

Replace the keyword **FUZZ** with values from a wordlist.

Example:

```bash
gobuster fuzz -u https://example.com/FUZZ -w wordlist.txt
```

Gobuster will test multiple values in place of **FUZZ**.

---

# Amazon S3 Enumeration

Purpose:

Search for publicly accessible Amazon S3 buckets.

Syntax:

```bash
gobuster s3 -w buckets.txt
```

---

# Google Cloud Storage Enumeration

Purpose:

Search for publicly accessible Google Cloud Storage buckets.

Syntax:

```bash
gobuster gcs -w buckets.txt
```

---

# Save Scan Results

Output can be saved into a text file.

```bash
-o results.txt
```

Example:

```bash
gobuster dir -u https://example.com -w wordlist.txt -o results.txt
```

---

# Increase Scan Speed

Use multiple threads:

```bash
-t 100
```

Higher thread counts can speed up scans but may increase server load.

---

# Scan Specific File Extensions

Example:

```bash
-x php,html,txt,js
```

Gobuster will check for files with the specified extensions.

---

# Ignore SSL Certificate Errors

```bash
-k
```

Useful when testing environments with self-signed certificates.

---

# Custom HTTP Header

Example:

```bash
-H "Authorization: Bearer TOKEN"
```

Useful for authenticated testing.

---

# Add Cookies

Example:

```bash
-c "PHPSESSID=YOUR_SESSION_ID"
```

Useful when testing authenticated areas.

---

# Random User-Agent

```bash
--random-agent
```

Uses a random browser User-Agent for requests.

---

# Show Help

```bash
gobuster --help
```

Displays all available modes and options.

---

# Check Version

```bash
gobuster version
```

Displays the installed Gobuster version.

---

# Best Practices

- Always use authorized targets.
- Select an appropriate wordlist for the target.
- Adjust thread count responsibly.
- Save scan results for later analysis.
- Review findings carefully before reporting them.

---

# Summary

Gobuster provides several powerful modes for enumeration. Understanding the purpose of each mode and its options helps security professionals perform efficient and organized reconnaissance during authorized penetration testing.
