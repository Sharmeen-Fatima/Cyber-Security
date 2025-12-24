# 📡 Ping Command Flags Explained (Windows)

This repository explains **Windows `ping` command flags** in a **simple and easy English way**, especially for beginners who want quick understanding.

---

## 🔹 What is Ping?

`ping` is a network command used to **check connectivity** between your computer and another device or server.

Example:

```cmd
ping google.com
```

---

## 🔹 Ping Command Flags (One-Line Explanation)

| Flag             | Explanation                                       |
| ---------------- | ------------------------------------------------- |
| `-t`             | Continuously pings the target until you stop it   |
| `-a`             | Resolves IP address into hostname                 |
| `-n count`       | Sends ping request a specific number of times     |
| `-l size`        | Sets the size of data sent in each ping           |
| `-f`             | Prevents packet from being fragmented (IPv4 only) |
| `-i TTL`         | Sets how many hops the packet can travel          |
| `-v TOS`         | Sets packet priority (deprecated, IPv4 only)      |
| `-r count`       | Records the route taken by the packet (IPv4 only) |
| `-s count`       | Adds timestamp for each hop (IPv4 only)           |
| `-j host-list`   | Packet loosely follows a specified route          |
| `-k host-list`   | Packet strictly follows a specified route         |
| `-w timeout`     | Time to wait for a reply (in milliseconds)        |
| `-R`             | Tests reverse route of packet (IPv6 only)         |
| `-S srcaddr`     | Uses a specific source IP address                 |
| `-c compartment` | Uses a specific network compartment               |
| `-p`             | Pings Hyper-V virtual network address             |
| `-4`             | Forces ping to use IPv4 only                      |
| `-6`             | Forces ping to use IPv6 only                      |

---

## 🔹 Example Commands

```cmd
ping google.com -n 5
```

➡ Sends 5 ping requests

```cmd
ping 8.8.8.8 -t
```

➡ Continuously pings until stopped

```cmd
ping google.com -4
```

➡ Forces IPv4 ping

---

## 🎯 Purpose of This Repo

* Help beginners understand `ping` command
* Simple explanations in **one line**
* Useful for **networking basics & troubleshooting**
