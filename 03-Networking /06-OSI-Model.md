# 📖 6. OSI Model (Open Systems Interconnection Model)

> "The OSI Model explains how data travels from one device to another over a network."

---

# 🎯 Learning Objectives

After completing this topic, you will:

- Understand what the OSI Model is.
- Learn why the OSI Model is important.
- Learn all 7 layers of the OSI Model.
- Understand the job of each layer.
- Learn how data travels across a network.

---

# 🤔 What is the OSI Model?

The **OSI Model (Open Systems Interconnection Model)** is a framework that explains **how data travels from one device to another over a network.**

Instead of doing everything at once, networking is divided into **7 layers**, and each layer has a specific job.

Think of it like sending a parcel.

You don't simply throw the parcel to your friend.

Instead, you:

- Pack the parcel.
- Write the address.
- Give it to the courier.
- The courier transports it.
- Your friend receives it.
- Opens the parcel.

Similarly, data passes through different layers before reaching the destination.

---

# ❓ Why Do We Need the OSI Model?

The OSI Model helps us:

- Understand how networking works.
- Troubleshoot network problems.
- Learn networking step by step.
- Understand where attacks happen.
- Build a strong networking foundation.

---

# 🏗 The 7 Layers of the OSI Model

```
+---------------------------+
| 7. Application            |
+---------------------------+
| 6. Presentation           |
+---------------------------+
| 5. Session                |
+---------------------------+
| 4. Transport              |
+---------------------------+
| 3. Network                |
+---------------------------+
| 2. Data Link              |
+---------------------------+
| 1. Physical               |
+---------------------------+
```

---

# 🎓 Easy Trick to Remember

From Top to Bottom

```
Application
Presentation
Session
Transport
Network
Data Link
Physical
```

### Mnemonic

> **All People Seem To Need Data Processing**

---

# 🌍 Imagine Sending a WhatsApp Message

When you send:

```
Hello 👋
```

The message doesn't instantly appear on your friend's phone.

It goes through several steps.

Those steps are explained by the **OSI Model**.

Let's understand each layer.

---

# 🌐 Layer 7 - Application Layer

### 📌 What does it do?

The **Application Layer** is the layer where users interact with applications and network services.

Whenever you:

- Open Google Chrome
- Watch YouTube
- Send an Email
- Use WhatsApp
- Browse Facebook

you are using the Application Layer.

---

### 🌍 Real-Life Example

Opening Chrome and visiting:

```
https://google.com
```

---

### 🌐 Common Protocols

- HTTP
- HTTPS
- FTP
- SMTP
- DNS

(Don't worry if these are new. You'll learn them later.)

---

### 🔐 Cybersecurity Importance

Most **Bug Bounty** and **Web Penetration Testing** vulnerabilities exist at this layer.

Examples:

- SQL Injection
- Cross-Site Scripting (XSS)
- Cross-Site Request Forgery (CSRF)
- Authentication Issues

---

# 🎨 Layer 6 - Presentation Layer

### 📌 What does it do?

The Presentation Layer prepares data before sending it.

Its main jobs are:

- Encryption
- Decryption
- Compression
- Formatting

Think of it like wrapping a gift before sending it.

---

### 🌍 Real-Life Example

When you visit:

```
https://example.com
```

your browser encrypts the communication.

---

### 🔐 Cybersecurity Importance

Encryption protects sensitive information while it travels across the network.

---

# 🤝 Layer 5 - Session Layer

### 📌 What does it do?

The Session Layer starts, manages, and ends communication between two devices.

Think of it like starting and ending a phone call.

---

### 🌍 Real-Life Example

- Joining a Zoom Meeting
- Leaving the Zoom Meeting

---

### 🔐 Cybersecurity Importance

Secure sessions help prevent attackers from hijacking active connections.

---

# 🚚 Layer 4 - Transport Layer

### 📌 What does it do?

The Transport Layer makes sure data reaches the destination correctly.

It controls how data is sent and received.

---

## Two Important Protocols

### TCP (Transmission Control Protocol)

- Reliable
- Checks for errors
- Resends lost data
- Slightly slower

Used for:

- Websites
- Banking
- Emails
- File Downloads

---

### UDP (User Datagram Protocol)

- Faster
- Doesn't check for errors
- Doesn't resend lost packets

Used for:

- Online Games
- Live Streaming
- Video Calls

---

### 🔐 Cybersecurity Importance

Many attacks and scans target this layer, such as:

- Port Scanning
- TCP SYN Scans
- UDP Scans

---

# 🛣 Layer 3 - Network Layer

### 📌 What does it do?

The Network Layer decides where data should go.

It uses **IP Addresses** to send data between different networks.

---

### 🌍 Real-Life Example

Just like your house has an address,

every device connected to the Internet has an IP Address.

---

### 🖥 Device

Router

---

### 🌐 Common Protocols

- IP
- ICMP

---

### 🔐 Cybersecurity Importance

SOC Analysts and Penetration Testers frequently analyze IP addresses, routing, and network traffic.

---

# 📦 Layer 2 - Data Link Layer

### 📌 What does it do?

The Data Link Layer delivers data between devices on the same local network.

It uses **MAC Addresses**.

---

### 🌍 Real-Life Example

Two computers connected to the same office switch.

---

### 🖥 Device

Switch

---

### 🔐 Cybersecurity Importance

Common attacks include:

- ARP Spoofing
- MAC Flooding

You'll learn these in later chapters.

---

# ⚡ Layer 1 - Physical Layer

### 📌 What does it do?

The Physical Layer sends data as electrical, radio, or light signals.

It includes:

- Ethernet Cables
- Fiber Optic Cables
- Wi-Fi Signals

Everything is transmitted as **Bits (0s and 1s).**

---

### 🌍 Real-Life Example

Connecting your laptop to a router using an Ethernet cable.

---

### 🖥 Devices

- Hub
- Repeater
- Cables

---

### 🔐 Cybersecurity Importance

Physical security is also important.

If an attacker gains physical access to a network, they may steal data or install malicious devices.

---

# 📊 OSI Model Summary

| Layer | Name | Main Job | Example |
|--------|------|----------|---------|
| 7 | Application | User interacts with applications | Chrome, Gmail |
| 6 | Presentation | Encrypts and formats data | HTTPS |
| 5 | Session | Starts and ends communication | Zoom |
| 4 | Transport | Reliable delivery of data | TCP, UDP |
| 3 | Network | Uses IP Address for routing | Router |
| 2 | Data Link | Uses MAC Address for local delivery | Switch |
| 1 | Physical | Sends bits through cables or Wi-Fi | Ethernet Cable |

---

# 🌍 How Data Travels

Imagine you open:

```
youtube.com
```

The request follows this path:

```
You

↓

Application

↓

Presentation

↓

Session

↓

Transport

↓

Network

↓

Data Link

↓

Physical

↓

🌐 Internet

↓

YouTube Server

↓

Physical

↓

Data Link

↓

Network

↓

Transport

↓

Session

↓

Presentation

↓

Application

↓

🎉 YouTube Opens
```

---

# 📝 Quick Notes

- OSI stands for **Open Systems Interconnection**.
- The OSI Model has **7 layers**.
- Each layer performs a specific task.
- Data moves from **Layer 7 → Layer 1** while sending.
- Data moves from **Layer 1 → Layer 7** while receiving.

---

# 💡 Interview Questions

### Q1. What does OSI stand for?

Open Systems Interconnection.

---

### Q2. How many layers are there in the OSI Model?

7 Layers.

---

### Q3. Which layer is closest to the user?

Application Layer.

---

### Q4. Which layer uses IP Addresses?

Network Layer.

---

### Q5. Which layer uses MAC Addresses?

Data Link Layer.

---

### Q6. Which layer is responsible for sending bits?

Physical Layer.

---

### Q7. Which protocols work at the Transport Layer?

TCP and UDP.

---

### Q8. Which device works at the Network Layer?

Router.

---

# 🎯 Mini Activity

1. Draw the seven OSI layers in your notebook.
2. Memorize the layer names using the mnemonic:
   - **All People Seem To Need Data Processing**
3. Think about what happens when you open a website and try to explain how the request moves through the seven layers.

---

# ✅ Checklist

- [ ] I know what the OSI Model is.
- [ ] I know why the OSI Model is important.
- [ ] I can name all 7 layers.
- [ ] I understand the purpose of each layer.
- [ ] I know how data travels through the OSI Model.
- [ ] I'm ready to learn the TCP/IP Model.
