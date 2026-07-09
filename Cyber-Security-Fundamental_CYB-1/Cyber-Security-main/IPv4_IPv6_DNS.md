# Cyber Security Fundamentals – IPv4, IPv6 & DNS.

## 🌐 Introduction

Whenever you browse the internet, watch YouTube, send a message on WhatsApp, or open any website, your computer uses several networking technologies behind the scenes.

In this lesson, we will learn:

* What is an IP Address?
* What is IPv4 Address Space?
* What is IPv6?
* IPv4 vs IPv6
* What is DNS (Domain Name System)?
* Practical Commands:

  * `ipconfig`
  * `ping`
  * `nslookup`

---

## 📌 What is an IP Address?

An **IP Address (Internet Protocol Address)** is a unique numerical address assigned to every device connected to a network.

It allows devices to identify and communicate with each other over the internet or a local network.

### 💡 Real-Life Example

Think of your home address.

When someone sends you a parcel, they need your home address so the parcel reaches the correct destination.

Similarly, every device connected to the internet needs an **IP Address** so data knows exactly where to go.

Without an IP address, devices cannot communicate with each other.

---

# IPv4 Address Space

## What is IPv4?

**IPv4 (Internet Protocol Version 4)** is the fourth version of the Internet Protocol and is still the most commonly used IP addressing system.

An IPv4 address is **32 bits long** and consists of **4 numbers (octets)** separated by dots (`.`).

### Example

```text
192.168.1.10
```

Each section is called an **Octet**.

```text
192 . 168 . 1 . 10
```

Each octet contains **8 bits**, which means every octet can have a value from:

```text
0 - 255
```

---

## Why is the Range 0–255?

Each octet contains **8 binary bits**.

The smallest binary value is:

```text
00000000 = 0
```

The largest binary value is:

```text
11111111 = 255
```

Therefore, every section of an IPv4 address can only contain numbers between **0 and 255**.

---

## What is Address Space?

**Address Space** means the total number of unique IP addresses that can be created.

Since IPv4 uses **32 bits**, the total number of possible addresses is:

```text
2³² = 4,294,967,296
```

Approximately:

**4.3 Billion IP Addresses**

---

## Why Was IPv4 Not Enough?

When the internet was first introduced, only a small number of computers were connected.

Today, billions of devices use the internet, including:

* Computers
* Laptops
* Smartphones
* Smart TVs
* CCTV Cameras
* Gaming Consoles
* Smart Watches
* IoT Devices
* Smart Home Appliances

Because of this rapid growth, IPv4 addresses started running out.

To solve this problem, **IPv6** was introduced.

---

# What is IPv6?

**IPv6 (Internet Protocol Version 6)** is the latest version of the Internet Protocol.

It was developed to replace IPv4 and provide a much larger number of IP addresses.

Unlike IPv4, IPv6 uses **128 bits**.

### Example

```text
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

IPv6 uses:

* Hexadecimal numbers (0-9 and A-F)
* Colons (`:`) instead of dots (`.`)

---

## Why Do We Need IPv6?

The internet continues to grow every day.

More devices require unique IP addresses than IPv4 can provide.

IPv6 offers an almost unlimited number of addresses, making it suitable for future technologies and the growing number of internet-connected devices.

### 💡 Real-Life Example

Imagine a city with only **4 billion house numbers**.

As the population grows, eventually there will be no new house numbers available.

Instead of expanding the existing city, a brand-new city with almost unlimited house numbers is built.

That new city is similar to **IPv6**.

---

# IPv4 vs IPv6

| Feature         | IPv4                        | IPv6                          |
| --------------- | --------------------------- | ----------------------------- |
| Full Form       | Internet Protocol Version 4 | Internet Protocol Version 6   |
| Address Length  | 32 bits                     | 128 bits                      |
| Address Format  | Decimal Numbers             | Hexadecimal Numbers           |
| Separator       | Dot (`.`)                   | Colon (`:`)                   |
| Example         | 192.168.1.1                 | 2001:db8::1                   |
| Total Addresses | About 4.3 Billion           | Approximately 340 Undecillion |
| Current Usage   | Most Common                 | Growing Rapidly               |
| Future Ready    | Limited                     | Yes                           |

---

# What is DNS (Domain Name System)?

DNS stands for **Domain Name System**.

DNS converts **domain names** into **IP addresses**.

Humans can easily remember website names, but computers communicate using IP addresses.

DNS works as a translator between humans and computers.

---

## 💡 Real-Life Example

Imagine you want to call your friend.

You search for your friend's **name** in your phone instead of remembering their phone number.

Your mobile phone automatically finds the correct number.

DNS works in the same way.

Instead of remembering:

```text
142.250.xxx.xxx
```

You simply type:

```text
www.google.com
```

DNS finds Google's IP address and connects you to the correct server.

---

## How DNS Works

### Step 1

You enter:

```text
www.google.com
```

⬇

### Step 2

Your computer sends a request to a DNS Server.

> "What is the IP address of [www.google.com](http://www.google.com)?"

⬇

### Step 3

The DNS Server finds the IP address.

⬇

### Step 4

The IP address is returned to your computer.

⬇

### Step 5

Your browser connects to Google's server and loads the website.

---

# 💻 Practical Commands

## 1️⃣ ipconfig

### Purpose

Displays your computer's network configuration.

### Syntax

```cmd
ipconfig
```

### Information You Can View

* IPv4 Address
* IPv6 Address
* Subnet Mask
* Default Gateway

### Example Output

```text
IPv4 Address . . . : 192.168.1.5

Subnet Mask . . . : 255.255.255.0

Default Gateway . : 192.168.1.1
```

---

## 2️⃣ ping

### Purpose

Checks whether another device or website is reachable over the network.

It is also used to test internet connectivity and measure response time.

### Syntax

```cmd
ping google.com
```

### Example Output

```text
Reply from 142.250.xxx.xxx

Bytes=32

Time=18ms

TTL=116
```

### Common Responses

✅ **Reply from...**

The destination is reachable.

❌ **Request Timed Out**

Possible reasons:

* No internet connection
* Server is offline
* Firewall is blocking requests
* Network connectivity issue

---

## 3️⃣ nslookup

### Purpose

Finds the IP address of a domain using DNS.

It is commonly used to verify DNS records and troubleshoot DNS-related issues.

### Syntax

```cmd
nslookup google.com
```

### Example Output

```text
Name: google.com

Address: 142.250.xxx.xxx
```

This shows that DNS successfully translated the domain name into its corresponding IP address.


---

> 💡 *This README is for educational purposes — designed to help beginners understand the core concepts of Cyber Security Fundamental clearly and professionally.*

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *09 July 2026*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Cyber Security Fundamental and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***
