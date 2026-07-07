# IP Address Fundamentals

## Introduction

Before learning Cyber Security, you need to understand one of the most important networking concepts: the **IP Address**.

Every device connected to a network or the internet needs an IP address so it can communicate with other devices.

Think of an IP address as a **home address** for your device. Just like a mail carrier needs your home address to deliver a package, the internet needs an IP address to send and receive data.

---

# What is an IP Address?

**IP** stands for **Internet Protocol**.

An **IP Address (Internet Protocol Address)** is a unique numerical address assigned to a device on a network.

It allows devices to:

- Identify each other
- Send data
- Receive data
- Communicate over a network or the internet

### Example

```text
192.168.1.10
```

```text
8.8.8.8
```

These numbers are examples of IPv4 addresses.

---

## Real-Life Example

Imagine you want to send a letter to your friend.

Without a home address, the post office would not know where to deliver it.

The internet works the same way.

```
Home Address
      ↓
123 Main Street
```

```
Internet
      ↓
IP Address
192.168.1.10
```

Every device has an address that helps data reach the correct destination.

---

# Types of IP Address

There are two main types of IP addresses.

## 1. Public IP Address

A **Public IP Address** is assigned to your internet connection.

It is visible on the internet and allows your network to communicate with websites and online services.

### Example

```text
103.25.80.5
```

When you visit Google, YouTube, or any website, they see your **public IP address**.

### Key Points

- Visible on the internet
- Assigned by your Internet Service Provider (ISP)
- Must be unique worldwide

---

## 2. Private IP Address

A **Private IP Address** is used inside a local network, such as your home, school, or office.

It is **not directly accessible from the internet**.

### Example

```text
192.168.1.2
192.168.1.3
192.168.1.4
```

Your router assigns private IP addresses to devices connected to your network.

### Home Network Example

```text
                Internet
                    │
              Public IP
                    │
                [ Router ]
                /    |    \
               /     |     \
         Laptop   Mobile    TV
      192.168.1.2
      192.168.1.3
      192.168.1.4
```

### Key Points

- Used inside local networks
- Assigned by the router
- Not visible on the public internet
- The same private IP ranges can be used in many different networks

---

# Public vs Private IP Address

| Public IP | Private IP |
|-----------|------------|
| Used on the internet | Used inside local networks |
| Visible to websites | Hidden from the internet |
| Assigned by an ISP | Assigned by a router |
| Must be globally unique | Can be reused in different networks |

---

# Who Assigns an IP Address?

Different organizations assign different types of IP addresses.

## Step 1: IANA

**IANA (Internet Assigned Numbers Authority)** manages the global pool of IP addresses.

---

## Step 2: Regional Internet Registries (RIRs)

IANA distributes IP address blocks to Regional Internet Registries (RIRs).

These organizations manage IP addresses for different parts of the world.

---

## Step 3: Internet Service Providers (ISPs)

Internet Service Providers receive IP address ranges from RIRs.

Examples include:

- PTCL
- StormFiber
- Nayatel
- Transworld

Your ISP assigns your **Public IP Address**.

---

## Step 4: Your Router

Inside your home or office, your router assigns **Private IP Addresses** to devices.

This process is usually done automatically using **DHCP (Dynamic Host Configuration Protocol)**.

---

# IPv4 Address Classes

IPv4 addresses were originally divided into five classes.

Each class was designed for different network sizes.

| Class | First Octet Range | Purpose |
|--------|-------------------|----------|
| A | 1 – 126 | Large networks |
| B | 128 – 191 | Medium-sized networks |
| C | 192 – 223 | Small networks |
| D | 224 – 239 | Multicast |
| E | 240 – 255 | Experimental |

---

## Class A

- First octet: **1 – 126**
- Designed for very large organizations

### Example

```text
10.1.2.3
```

Structure

```text
Network.Host.Host.Host
```

---

## Class B

- First octet: **128 – 191**
- Designed for medium-sized organizations

### Example

```text
172.16.5.8
```

Structure

```text
Network.Network.Host.Host
```

---

## Class C

- First octet: **192 – 223**
- Designed for small organizations and home networks

### Example

```text
192.168.1.5
```

Structure

```text
Network.Network.Network.Host
```

---

## Class D

- First octet: **224 – 239**
- Used for **Multicast** communication

Instead of sending data to one device, multicast sends data to multiple devices at the same time.

Example:

- Live video streaming
- Online conferences
- IPTV

---

## Class E

- First octet: **240 – 255**
- Reserved for research and experimental purposes
- Not used for normal communication on the internet

---

# Quick Summary

- An **IP Address** is a unique address used to identify a device on a network.
- **Public IP Addresses** are used on the internet and are assigned by an **ISP**.
- **Private IP Addresses** are used inside local networks and are assigned by a **router**.
- **IANA** manages global IP addresses.
- **RIRs** distribute IP addresses to Internet Service Providers.
- IPv4 addresses are divided into **Class A, B, C, D, and E**, based on network size and purpose.

---

# Key Takeaways

- Every device needs an IP address to communicate.
- Public IP addresses connect your network to the internet.
- Private IP addresses allow devices to communicate inside a local network.
- Routers assign private IP addresses using DHCP.
- Understanding IP addressing is a fundamental networking skill and an essential foundation for Cyber Security.


---

> 💡 *This README is for educational purposes — designed to help beginners understand the core concepts of Cyber Security Fundamental clearly and professionally.*

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *07 June 2026*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Cyber Security Fundamental and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***


