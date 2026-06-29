# Gobuster Practical Examples

## 📌 Introduction

This document contains practical Gobuster examples to help beginners understand how different modes and options work.

> **Disclaimer:** These examples are intended for educational purposes and authorized security assessments only.

---

# Example 1 – Basic Directory Enumeration

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt
```

### Purpose

Searches for hidden directories and files using the provided wordlist.

---

# Example 2 – Save Results to a File

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -o results.txt
```

### Purpose

Stores the scan results in a text file for later review.

---

# Example 3 – Scan for Multiple File Extensions

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -x php,html,txt
```

### Purpose

Checks common file extensions while performing directory enumeration.

---

# Example 4 – Increase Scan Speed

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -t 50
```

### Purpose

Uses multiple threads to perform requests more efficiently.

---

# Example 5 – DNS Enumeration

### Command

```bash
gobuster dns -d example.com -w subdomains.txt
```

### Purpose

Attempts to discover subdomains listed in the wordlist.

---

# Example 6 – Display IP Addresses

### Command

```bash
gobuster dns -d example.com -w subdomains.txt -i
```

### Purpose

Shows the resolved IP address for discovered subdomains.

---

# Example 7 – Virtual Host Enumeration

### Command

```bash
gobuster vhost -u https://example.com -w wordlist.txt
```

### Purpose

Searches for virtual hosts configured on the target web server.

---

# Example 8 – Ignore SSL Certificate Errors

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -k
```

### Purpose

Allows scanning when the server uses a self-signed or otherwise untrusted SSL certificate.

---

# Example 9 – Add a Custom Header

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -H "Authorization: Bearer YOUR_TOKEN"
```

### Purpose

Adds a custom HTTP header to each request.

---

# Example 10 – Send Session Cookies

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt -c "SESSION=YOUR_SESSION_ID"
```

### Purpose

Uses an authenticated session cookie when testing authorized areas of a web application.

---

# Example 11 – Random User-Agent

### Command

```bash
gobuster dir -u https://example.com -w wordlist.txt --random-agent
```

### Purpose

Sends requests using a randomly selected User-Agent.

---

# Example 12 – Fuzz Mode

### Command

```bash
gobuster fuzz -u https://example.com/FUZZ -w wordlist.txt
```

### Purpose

Replaces the keyword **FUZZ** with entries from the wordlist.

---

# Example 13 – View Help

### Command

```bash
gobuster --help
```

### Purpose

Displays available commands, modes, and options.

---

# Example 14 – Check Installed Version

### Command

```bash
gobuster version
```

### Purpose

Displays the installed version of Gobuster.

---

# Example 15 – Basic Output Example

Example output:

```text
===============================================================
Gobuster v3.x
===============================================================

Found: /admin
Found: /login
Found: /images
Found: /robots.txt
```

### Explanation

Each "Found" entry indicates that the server responded positively for that resource, meaning it exists and is accessible.

---

# Best Practices

* Use Gobuster only on systems you own or have permission to test.
* Choose the appropriate mode for your objective.
* Select a suitable wordlist.
* Save important scan results.
* Review findings carefully before reporting them.

---

# Summary

These examples demonstrate common Gobuster commands used during authorized reconnaissance and enumeration. Understanding these examples provides a solid foundation for learning how Gobuster is used in ethical hacking and penetration testing.
