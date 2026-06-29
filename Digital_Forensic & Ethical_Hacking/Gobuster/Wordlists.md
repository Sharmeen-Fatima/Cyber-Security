# Wordlists in Gobuster

## 📌 Introduction

A wordlist is a text file that contains a collection of words or paths. Gobuster reads each word from the file and tests it against the target during enumeration.

Wordlists are one of the most important components of Gobuster because the quality of a scan depends heavily on the selected wordlist.

---

# What is a Wordlist?

A wordlist is simply a plain text (`.txt`) file where each line contains one word.

Example:

```text
admin
login
dashboard
backup
config
images
uploads
test
```

During a directory scan, Gobuster combines each word with the target URL.

Example:

Target:

```
https://example.com
```

Gobuster will test:

```
https://example.com/admin
https://example.com/login
https://example.com/dashboard
https://example.com/backup
https://example.com/config
```

If a resource exists, Gobuster reports it in the output.

---

# Why Are Wordlists Important?

The effectiveness of a Gobuster scan depends largely on the wordlist being used.

A good wordlist can help discover:

- Hidden directories
- Login pages
- Administrative panels
- Backup files
- Configuration files
- API endpoints
- Development folders
- Test environments

A poor or unrelated wordlist may miss important resources.

---

# Types of Wordlists

Different tasks require different wordlists.

## 1. Directory Wordlists

Used to discover hidden folders and web pages.

Example entries:

```text
admin
uploads
backup
images
private
portal
```

---

## 2. File Wordlists

Used to discover specific files.

Example entries:

```text
config
robots
index
backup
database
```

Often combined with file extensions such as:

```
.php
.html
.txt
.bak
.zip
```

---

## 3. Subdomain Wordlists

Used with DNS mode.

Example entries:

```text
mail
api
dev
test
vpn
blog
```

Gobuster checks whether these subdomains exist.

---

## 4. Virtual Host Wordlists

Used in VHOST mode.

Example entries:

```text
admin
internal
portal
stage
beta
```

---

# Small vs Large Wordlists

## Small Wordlists

Advantages:

- Faster scans
- Lower bandwidth usage
- Good for quick assessments

Disadvantages:

- May miss uncommon resources

---

## Large Wordlists

Advantages:

- Better coverage
- Higher chance of finding hidden content

Disadvantages:

- Slower scans
- More requests sent to the target
- Longer completion time

---

# Choosing the Right Wordlist

The best wordlist depends on your goal.

| Objective | Recommended Wordlist Type |
|------------|---------------------------|
| Directory discovery | Directory wordlist |
| File discovery | File wordlist |
| Subdomain discovery | DNS wordlist |
| Virtual host discovery | VHOST wordlist |

---

# Popular Wordlist Collections

The cybersecurity community commonly uses collections such as:

- SecLists
- DirBuster Wordlists
- Assetnote Wordlists
- FuzzDB

Each collection is designed for different enumeration scenarios.

---

# Tips for Better Results

- Start with a small wordlist for quick reconnaissance.
- Use larger wordlists when performing a more thorough assessment.
- Match the wordlist to the type of scan.
- Keep your wordlists organized.
- Update your wordlists regularly.

---

# Creating Your Own Wordlist

You can also create a custom wordlist tailored to your target.

Example:

```text
admin
staff
employee
portal
dashboard
backup
old
beta
```

Custom wordlists are useful for internal security assessments and authorized testing.

---

# Best Practices

- Choose a wordlist appropriate for the scan type.
- Avoid unnecessarily large wordlists for simple tasks.
- Combine wordlists with suitable file extensions when needed.
- Review scan results carefully before drawing conclusions.

---

# Summary

Wordlists are the foundation of Gobuster. Selecting the right wordlist improves scan efficiency and increases the likelihood of discovering useful resources during authorized security assessments.

---

> 💡 *This README is for educational purposes — designed to help beginners understand the core concepts of Digital_Forensic & Ethical_Hacking clearly and professionally.*

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *29 June 2026*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Digital_Forensic & Ethical_Hacking and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***


