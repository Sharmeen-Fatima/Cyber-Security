# 🌐 Tracert Command Explained (Windows)

This repository explains the **Windows `tracert` command** and its flags in **simple English**, specially for **Cyber Security Fundamentals students**.

---

## 🔹 What is Tracert?

`tracert` (Trace Route) is a network command used to **show the path (hops)** that packets take to reach a destination.

Example:

```cmd
tracert google.com
```

---

## 🔹 Tracert Command Flags (One-Line Explanation)

| Flag              | Explanation                                                |
| ----------------- | ---------------------------------------------------------- |
| `-d`              | Does not resolve IP addresses to hostnames (faster output) |
| `-h maximum_hops` | Sets the maximum number of hops to reach the target        |
| `-j host-list`    | Packet loosely follows a specified route (IPv4 only)       |
| `-w timeout`      | Time to wait for each hop reply (in milliseconds)          |
| `-R`              | Traces forward and return path of packet (IPv6 only)       |
| `-S srcaddr`      | Uses a specific source IPv6 address                        |
| `-4`              | Forces tracert to use IPv4 only                            |
| `-6`              | Forces tracert to use IPv6 only                            |

---

## 🔹 Example Commands

```cmd
tracert google.com
```

➡ Shows all network hops to Google

```cmd
tracert google.com -d
```

➡ Faster result without hostname resolution

```cmd
tracert google.com -h 10
```

➡ Limits tracing to 10 hops only

```cmd
tracert google.com -4
```

➡ Forces IPv4 tracing

---

## 🔐 Cyber Security Importance

* Helps identify **network path & routing issues**
* Useful for detecting **packet delays, drops, or suspicious hops**
* Commonly used in **network troubleshooting & reconnaissance**

---

## 🎯 Purpose of This Repository

* Learn `tracert` command basics
* Understand how packets travel in a network
* Build strong foundation for **Cyber Security & Networking**

---

🧠 **Author:** *[Sharmeen Fatima](https://github.com/sharmeen-fatima)*  
📅 **Last Updated:** *11 November 2025*  

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Cyber-Security and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***

