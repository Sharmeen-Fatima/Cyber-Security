# 🐧 Kali Linux Installation Guide for Beginners

## 📖 What is Linux?

**Linux** is an open-source operating system just like Windows and macOS. It is widely used by developers, cybersecurity professionals, and system administrators.

### 💡 Why do we use Linux?

* Free and open-source
* More secure than many other operating systems
* Highly customizable
* Widely used in **cybersecurity and ethical hacking**
* Supports powerful command-line tools

👉 Kali Linux is a special Linux distribution used for **penetration testing and security learning**.

---

## 💻 System Requirements

Before starting, make sure your system meets the following minimum requirements:

### ✅ Required Configuration:

* **RAM:** 8 GB (16 GB recommended for better performance)
* **Storage:** 256 GB (SSD / M.2 / HDD)
* **Processor:** Intel Core i3 or above (latest generation preferred)
* **Virtualization:** Must be enabled

---

## 📌 Introduction

Before installing Kali Linux, it is important to understand the two common methods:

### 1. Dual Boot (Advanced Users)

Dual Boot allows you to install **Windows and Linux on the same machine**.

* You can use **only one Operating System at a time**
* You must **restart your PC** to switch between Windows and Linux
* More suitable for **professionals and advanced users**
* Requires disk partitioning and careful setup

👉 Not recommended for beginners.

---

### 2. Virtual Machine (Recommended for Students)

A Virtual Machine allows you to run Linux **inside Windows**.

* No need to restart your PC
* Easy to install and manage
* Safe for beginners
* Both systems can run at the same time

👉 We will use this method in this guide.


Got it — you want a clean, professional, beginner-friendly GitHub README that teaches students how to install Kali Linux using VirtualBox, with a short explanation of dual boot vs virtualization.

Here’s a complete repo-ready README you can copy and push 👇

---

# 🐧 Kali Linux Installation Guide for Beginners

This repository is designed to help students install **Kali Linux** step by step using **VirtualBox** in a simple and beginner-friendly way.

---

## 📌 Introduction

Before installing Kali Linux, it is important to understand the two common methods:

### 1. Dual Boot (Advanced Users)

Dual Boot allows you to install **Windows and Linux on the same machine**.

* You can use **only one Operating System at a time**
* You must **restart your PC** to switch between Windows and Linux
* More suitable for **professionals and advanced users**
* Requires disk partitioning and careful setup

👉 Not recommended for beginners.

---

### 2. Virtual Machine (Recommended for Students)

A Virtual Machine allows you to run Linux **inside Windows**.

* No need to restart your PC
* Easy to install and manage
* Safe for beginners
* Both systems can run at the same time

👉 We will use this method in this guide.

---

## 🧰 Required Software

Download all tools from their official websites:

1. VirtualBox
   [https://www.virtualbox.org/](https://www.virtualbox.org/)

2. Kali Linux ISO
   [https://www.kali.org/get-kali/#kali-platforms](https://www.kali.org/get-kali/#kali-platforms)

3. Visual Studio Code (Optional but Recommended)
   [https://code.visualstudio.com/](https://code.visualstudio.com/)

---

## ⚙️ Installation Overview

After downloading everything, we will install Kali Linux in **5 simple steps**:

1. Install VirtualBox
2. Enable Virtualization
3. Create Virtual Machine
4. Attach Kali Linux ISO
5. Configure and Install Kali Linux

---

## 🚀 Step-by-Step Installation

### ✅ Step 1: Install VirtualBox

* Download VirtualBox from the official website
* Run the installer
* Install with default settings

---

### ✅ Step 2: Enable Virtualization

Virtualization must be enabled on your system.

#### 🔍 Check from Task Manager:

1. Press `Ctrl + Shift + Esc`
2. Go to **Performance Tab**
3. Click on **CPU**
4. Look for **Virtualization**

👉 If it says **Enabled** → Good to go
👉 If Disabled → Enable it from BIOS

#### ⚠️ Enable from BIOS:

* Restart your PC
* Enter BIOS (usually `F2`, `Delete`, or `Esc`)
* Find **Virtualization Technology**
* Enable it and save changes

---

### ✅ Step 3: Create Virtual Machine

1. Open VirtualBox
2. Click **New**
3. Fill details:

* Name: `Kali Linux`
* Type: `Linux`
* Version: `Debian (64-bit)`

4. Set Memory (RAM):

   * Minimum: 2 GB
   * Recommended: 4 GB

5. Create Virtual Hard Disk:

   * Type: VDI
   * Storage: Dynamically Allocated
   * Size: 20 GB (minimum)

---

### ✅ Step 4: Attach Kali Linux ISO

1. Select your Virtual Machine
2. Click **Settings**
3. Go to **Storage**
4. Under Controller IDE → Click Empty
5. Click disk icon → **Choose a disk file**
6. Select downloaded Kali Linux ISO file

---

### ✅ Step 5: Configuration & Installation

1. Click **Start**

2. Kali Linux installer will open

3. Select:

   * Graphical Install (Recommended)

4. Follow on-screen instructions:

   * Language
   * Location
   * Keyboard layout
   * Username & Password

5. Wait for installation to complete

---

## 💻 After Installation

* Remove ISO file (optional)
* Restart Virtual Machine
* Login using your credentials

---

## 🧑‍💻 Optional: Install VS Code

You can install **VS Code** inside Kali Linux for coding practice.

---

## 🎯 Final Notes

* Always download files from official websites
* Do not rush BIOS settings
* Minimum system requirements:

  * 8 GB RAM recommended
  * SSD preferred

---

## 📚 Learning Outcome

After completing this guide, students will be able to:

* Understand Dual Boot vs Virtual Machine
* Install VirtualBox
* Set up Kali Linux safely
* Work in a Linux environment

