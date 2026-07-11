# 📖 8. IP Addressing (Internet Protocol Address)

> "An IP Address is like the home address of a device on a network."

---

# 🎯 Learning Objectives

After completing this topic, you will:

- Understand what an IP Address is.
- Learn why IP Addresses are important.
- Understand IPv4 and IPv6.
- Learn Public and Private IP Addresses.
- Understand Static and Dynamic IP Addresses.
- Learn basic IP Address classes.
- Understand how cybersecurity professionals use IP Addresses.

---

# 🤔 What is an IP Address?

An **IP Address (Internet Protocol Address)** is a unique number assigned to every device connected to a network.

Just like every house has an address,

every computer, mobile phone, server, printer, or router has an IP Address.

Without an IP Address, devices would not know where to send or receive data.

---

# 🌍 Real-Life Example

Imagine you want to send a letter to your friend.

The post office needs your friend's home address.

Without the address,

the letter cannot be delivered.

Similarly,

when you open

```
google.com
```

your computer sends a request to Google's IP Address.

Without an IP Address,

the data would never reach Google.

---

# ❓ Why Do We Need IP Addresses?

IP Addresses help devices:

- Identify each other.
- Send data.
- Receive data.
- Communicate over the Internet.

Without IP Addresses,

the Internet would not work.

---

# 🌐 Types of IP Addresses

There are two main versions:

## 1. IPv4

IPv4 is the most commonly used IP Address.

Example:

```
192.168.1.10
```

IPv4 contains **4 numbers** separated by dots.

Each number ranges from **0 to 255**.

Example:

```
192.168.0.1
```

---

## 2. IPv6

IPv6 was introduced because the Internet needed more IP Addresses.

Example:

```
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

IPv6 is much longer than IPv4.

It provides almost unlimited IP Addresses.

---

# 📊 IPv4 vs IPv6

| IPv4 | IPv6 |
|-------|-------|
| 32-bit Address | 128-bit Address |
| Uses dots (.) | Uses colons (:) |
| Limited addresses | Huge number of addresses |
| Example: 192.168.1.1 | Example: 2001:db8::1 |

---

# 🌍 Public IP Address

A **Public IP Address** is assigned by your Internet Service Provider (ISP).

It is visible on the Internet.

Example:

```
49.36.xx.xx
```

Your Public IP allows your home network to communicate with websites and online services.

---

# 🏠 Private IP Address

A **Private IP Address** is used inside a local network.

It is **not directly accessible from the Internet**.

Examples:

```
192.168.1.10

10.0.0.25

172.16.5.100
```

Most home Wi-Fi devices use Private IP Addresses.

---

# 🌍 Public vs Private IP

| Public IP | Private IP |
|------------|------------|
| Visible on the Internet | Used inside local networks |
| Assigned by ISP | Assigned by Router |
| Globally Unique | Can be reused in different networks |

---

# 🔄 Static IP Address

A **Static IP Address** never changes.

It remains the same every time the device connects.

Used for:

- Servers
- CCTV Systems
- Web Hosting

---

# 🔁 Dynamic IP Address

A **Dynamic IP Address** changes automatically.

It is assigned by **DHCP**.

Most home Internet users use Dynamic IP Addresses.

---

# 📊 Static vs Dynamic IP

| Static IP | Dynamic IP |
|------------|-------------|
| Doesn't change | Changes automatically |
| Manual configuration | Assigned by DHCP |
| Mostly servers | Home users |

---

# 📚 IPv4 Classes

| Class | Range | Used For |
|--------|-------|-----------|
| A | 1.0.0.0 - 126.255.255.255 | Large Networks |
| B | 128.0.0.0 - 191.255.255.255 | Medium Networks |
| C | 192.0.0.0 - 223.255.255.255 | Small Networks |
| D | 224.0.0.0 - 239.255.255.255 | Multicast |
| E | 240.0.0.0 - 255.255.255.255 | Research |

*(Don't worry about memorizing all of these right now. You'll use Classes A, B, and C most often.)*

---

# 🖥 How to Find Your IP Address

## Windows

Open Command Prompt.

Run:

```cmd
ipconfig
```

---

## Linux

Open Terminal.

Run:

```bash
ip addr
```

or

```bash
hostname -I
```

---

# 🔐 Cybersecurity Importance

Understanding IP Addresses is essential for:

### SOC Analyst

- Tracking attackers
- Investigating logs
- Detecting suspicious IPs
- Blocking malicious IPs

---

### Penetration Tester

- Scanning networks
- Finding live hosts
- Enumerating devices

---

### Bug Bounty Hunter

- Identifying target servers
- Testing APIs
- Investigating exposed services

---

# 🌍 Real-Life Scenario

When you open:

```
youtube.com
```

Your computer:

1. Finds YouTube's IP Address.
2. Sends a request.
3. Receives a response.
4. Loads the website.

All of this happens using IP Addresses.

---

# 📝 Quick Notes

- Every device on a network has an IP Address.
- IPv4 uses 32 bits.
- IPv6 uses 128 bits.
- Public IPs are visible on the Internet.
- Private IPs are used inside local networks.
- Static IPs do not change.
- Dynamic IPs are assigned automatically.

---

# 💡 Interview Questions

### Q1. What is an IP Address?

A unique address used to identify a device on a network.

---

### Q2. What is the difference between IPv4 and IPv6?

IPv4 uses 32-bit addresses with dots, while IPv6 uses 128-bit addresses with colons and provides many more unique addresses.

---

### Q3. What is the difference between a Public IP and a Private IP?

A Public IP is visible on the Internet and assigned by an ISP, while a Private IP is used only within a local network and assigned by a router.

---

### Q4. What is the difference between a Static IP and a Dynamic IP?

A Static IP remains the same, while a Dynamic IP is assigned automatically by DHCP and can change.

---

### Q5. Which command shows your IP Address in Windows?

```cmd
ipconfig
```

---

### Q6. Which command shows your IP Address in Linux?

```bash
ip addr
```

or

```bash
hostname -I
```

---

# 🎯 Mini Activity

1. Find your computer's IP Address.
2. Find your phone's IP Address.
3. Check whether they are Public or Private IP Addresses.
4. Write them in your notebook.

---

# ✅ Checklist

- [ ] I know what an IP Address is.
- [ ] I know why IP Addresses are important.
- [ ] I understand IPv4 and IPv6.
- [ ] I know the difference between Public and Private IPs.
- [ ] I know the difference between Static and Dynamic IPs.
- [ ] I know how to check my IP Address on Windows and Linux.
