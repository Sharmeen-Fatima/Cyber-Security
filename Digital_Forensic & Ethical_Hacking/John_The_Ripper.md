# John The Ripper

A beginner-friendly guide to using **John the Ripper** for password recovery on ZIP files in Kali Linux.

> **Disclaimer**
> This project is for educational purposes only. Use John the Ripper only on files and systems that you own or have permission to test.

---

# What is John the Ripper?

John the Ripper is a popular password recovery tool used by cybersecurity professionals and students. It helps recover passwords from different file formats by testing passwords from a wordlist or using other cracking methods.

---

# Requirements

- Kali Linux
- John the Ripper (Jumbo Version)
- RockYou Wordlist
- Password-Protected ZIP File

---

# Check if John the Ripper is Installed

```bash
john --version
```

If the version is displayed, John the Ripper is installed successfully.

---

# Check the RockYou Wordlist

```bash
ls /usr/share/wordlists/
```

If `rockyou.txt.gz` is available, unzip it:

```bash
gunzip /usr/share/wordlists/rockyou.txt.gz
```

---

# Go to the Folder

Move to the folder where your ZIP file is stored.

```bash
cd ~/Desktop
```

---

# Generate the Password Hash

Extract the password hash from the ZIP file.

```bash
zip2john Securet.zip > pass.hash
```

View the generated hash:

```bash
cat pass.hash
```

---

# Crack the Password

Use the RockYou wordlist to recover the password.

```bash
john pass.hash --wordlist=/usr/share/wordlists/rockyou.txt
```

---

# Display the Recovered Password

```bash
john --show pass.hash
```

Example Output:

```text
Securet.zip:123
```

---

# Common Commands

Check John Version

```bash
john --version
```

Generate ZIP Hash

```bash
zip2john Securet.zip > pass.hash
```

View Hash

```bash
cat pass.hash
```

Start Password Recovery

```bash
john pass.hash --wordlist=/usr/share/wordlists/rockyou.txt
```

Show Recovered Password

```bash
john --show pass.hash
```

---

# Common Errors

## Error

```text
No password hashes loaded
```

### Possible Reasons

- The hash file is empty.
- The ZIP file is not password protected.
- The ZIP file contains an empty file.
- The hash was not generated successfully.

---

## Error

```text
Securet.zip : No such file or directory
```

### Solution

Go to the correct folder.

```bash
cd ~/Desktop
```

---

## Error

```text
Skipping short file
```

### Solution

The encrypted file is too small or empty.

Add some content to the file, create the password-protected ZIP again, and generate the hash again.

---

# Project Structure

```
John-The-Ripper/
│
├── Securet.zip
├── pass.hash
└── README.md
```

---

# Learning Outcome

After completing this project, you will learn how to:

- Install and verify John the Ripper
- Generate a password hash from a ZIP file
- Use the RockYou wordlist
- Recover ZIP passwords
- Troubleshoot common errors


---

> 💡 *This README is for educational purposes — designed to help beginners understand the core concepts of Digital_Forensic & Ethical_Hacking clearly and professionally.*

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *27 June 2026*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Digital_Forensic & Ethical_Hacking and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***
