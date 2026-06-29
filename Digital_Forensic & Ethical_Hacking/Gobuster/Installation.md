# Gobuster Installation Guide

## 📌 Introduction

Gobuster is a command-line tool written in Go that is used for directory, DNS, virtual host, and cloud storage enumeration during authorized security assessments.

This guide explains how to install Gobuster on different operating systems.

---

# System Requirements

Before installing Gobuster, ensure that your system meets the following requirements:

- Windows, Linux, or macOS
- Internet connection
- Terminal or Command Prompt
- Go (only if building from source)

---

# Installation on Kali Linux

Gobuster comes pre-installed on many versions of Kali Linux.

To check whether it is installed:

```bash
gobuster --help
```

If Gobuster is not installed, update your packages:

```bash
sudo apt update
```

Install Gobuster:

```bash
sudo apt install gobuster
```

Verify installation:

```bash
gobuster version
```

---

# Installation on Ubuntu / Debian

Update package list:

```bash
sudo apt update
```

Install Gobuster:

```bash
sudo apt install gobuster
```

Verify installation:

```bash
gobuster version
```

---

# Installation on Windows

### Method 1 (Recommended)

1. Download the latest Gobuster release from the official GitHub repository.
2. Extract the ZIP file.
3. Place the executable in a preferred folder.
4. Add the folder to the Windows PATH environment variable.
5. Open Command Prompt or PowerShell.
6. Verify installation:

```powershell
gobuster version
```

---

# Installation using Go

If Go is installed on your system, run:

```bash
go install github.com/OJ/gobuster/v3@latest
```

After installation, verify:

```bash
gobuster version
```

---

# Verify Successful Installation

Run:

```bash
gobuster --help
```

If installed successfully, Gobuster will display its help menu and available commands.

---

# Common Installation Issues

### Command Not Found

Cause:
- Gobuster is not installed.
- PATH variable is not configured.

Solution:
- Reinstall Gobuster.
- Restart the terminal.
- Verify the installation path.

---

### Permission Denied

Cause:
- Insufficient permissions.

Solution:

```bash
sudo apt install gobuster
```

---

### Outdated Package

If your installed version is old:

```bash
sudo apt update
sudo apt upgrade gobuster
```

---

# Check Installed Version

```bash
gobuster version
```

Example Output:

```
Gobuster v3.x.x
```

---

# Next Step

After installing Gobuster successfully, continue with **Commands.md** to learn the basic syntax and commonly used commands.
