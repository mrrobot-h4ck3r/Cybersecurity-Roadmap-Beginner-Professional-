# 📖 Networking Essentials

> "Networking Essentials covers the core concepts that every beginner should know before learning Wireshark, Nmap, SOC Analysis, Penetration Testing, or Bug Bounty Hunting."

---

# 🎯 Learning Objectives

After completing this chapter, you will:

- Understand what a MAC Address is.
- Learn the difference between MAC Address and IP Address.
- Learn what Ports and Protocols are.
- Understand DNS, DHCP, NAT, and Subnetting.
- Learn important networking commands.
- Get introduced to Wireshark and Nmap.
- Understand basic Network Security concepts.

---

# 📍 1. MAC Address (Media Access Control Address)

## 🤔 What is a MAC Address?

A **MAC Address (Media Access Control Address)** is a **unique physical address** assigned to every network device.

Think of it as the **identity card** of your device.

Every laptop, computer, mobile phone, printer, router, and network card has its own MAC Address.

Unlike an IP Address, a MAC Address is assigned by the **manufacturer** and is stored in the device's Network Interface Card (NIC).

---

## ❓ Why Do We Need a MAC Address?

Imagine a classroom where every student has a unique roll number.

Even if two students have the same name, their roll numbers are different.

Similarly,

every device has its own MAC Address so it can be identified inside a local network.

Without MAC Addresses,

devices on the same network wouldn't know exactly which device should receive the data.

---

## 🌍 Real-Life Example

Suppose your home Wi-Fi has:

- Laptop
- Mobile Phone
- Smart TV
- Printer

All of them have different IP Addresses.

But they also have different MAC Addresses.

When your laptop sends data to your printer,

your Wi-Fi router or switch uses the **MAC Address** to make sure the data reaches the correct device.

---

# 📌 What Does a MAC Address Look Like?

Example:

```
00:1A:2B:3C:4D:5E
```

Another Example:

```
F4:5C:89:AB:12:34
```

A MAC Address contains **12 hexadecimal characters**.

Hexadecimal characters use:

```
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

They are usually written in pairs separated by colons (`:`) or hyphens (`-`).

Example:

```
00:15:5D:AA:BC:10
```

or

```
00-15-5D-AA-BC-10
```

Both represent the same type of MAC Address.

---

# 🖥 Where is a MAC Address Stored?

The MAC Address is stored inside the **Network Interface Card (NIC)**.

Every network device has a NIC.

Examples:

- Laptop Wi-Fi Card
- Ethernet Card
- Mobile Wi-Fi Chip
- Router Network Port

---

# 🌍 MAC Address vs IP Address

Many beginners confuse these two.

Think of it like this:

Your **house address** can change if you move to another city.

But your **Aadhaar Number** stays the same.

Similarly,

An IP Address can change.

A MAC Address usually stays the same.

---

| MAC Address | IP Address |
|-------------|------------|
| Physical Address | Logical Address |
| Assigned by Manufacturer | Assigned by Router or ISP |
| Usually doesn't change | Can change |
| Used inside a Local Network (LAN) | Used to communicate across networks and the Internet |
| Example: 00:1A:2B:3C:4D:5E | Example: 192.168.1.10 |

---

# 🏠 Where is a MAC Address Used?

MAC Addresses are mainly used inside a **Local Area Network (LAN)**.

For example:

- Home Wi-Fi
- Office Network
- School Network
- College Lab

Once data leaves your local network and travels across the Internet,

IP Addresses become more important.

---

# 📝 How a MAC Address Works

Imagine you want to send a file from your laptop to your printer.

The process looks like this:

```
Laptop

↓

Looks for Printer's MAC Address

↓

Switch/Wi-Fi Router finds the Printer

↓

File is delivered to the Printer

↓

Printing Starts
```

The switch uses the MAC Address to identify the correct device.

---

# 🔍 How to Find Your MAC Address

## Windows

Open **Command Prompt** and run:

```cmd
ipconfig /all
```

Look for:

```
Physical Address
```

Example Output:

```
Physical Address . . . . . : 34-17-EB-1A-5C-22
```

---

## Linux

Open Terminal.

Run:

```bash
ip addr
```

Example Output:

```text
link/ether 08:00:27:5A:9B:12
```

The value after **link/ether** is your MAC Address.

---

# 🔐 Cybersecurity Importance

### 👨‍💻 SOC Analyst

A SOC Analyst may:

- Investigate unknown devices on the network.
- Detect MAC Address spoofing.
- Monitor suspicious network activity.

---

### 🛡 Penetration Tester

A Penetration Tester uses MAC Addresses to:

- Discover devices.
- Perform network reconnaissance.
- Test Layer 2 attacks.

---

### 🐞 Bug Bounty Hunter

Bug bounty hunters usually focus on web applications.

However,

understanding MAC Addresses helps build a strong networking foundation.

---

# ⚠ MAC Address Spoofing

Sometimes attackers change their MAC Address to pretend to be another device.

This is called **MAC Address Spoofing**.

Example:

An attacker changes their laptop's MAC Address to match an authorized device on the network.

This may help them bypass certain network restrictions.

---

# 📝 Quick Notes

- MAC stands for **Media Access Control**.
- Every network device has a MAC Address.
- A MAC Address is a Physical Address.
- It is stored in the Network Interface Card (NIC).
- It is mainly used inside Local Area Networks (LAN).
- A MAC Address is different from an IP Address.
- Attackers can perform MAC Address Spoofing.

---

# 💡 Interview Questions

### Q1. What is a MAC Address?

A MAC Address is a unique physical address assigned to a network device.

---

### Q2. What does MAC stand for?

Media Access Control.

---

### Q3. Is a MAC Address Physical or Logical?

Physical Address.

---

### Q4. Which device stores the MAC Address?

The Network Interface Card (NIC).

---

### Q5. Can two devices have the same MAC Address?

Normally, no. Manufacturers assign unique MAC Addresses to devices.

---

### Q6. What is MAC Address Spoofing?

Changing a device's MAC Address to impersonate another device.

---

# 🎯 Mini Activity

1. Find your laptop's MAC Address.
2. Find your phone's MAC Address.
3. Compare both addresses.
4. Notice that they are different.

---

# ✅ Checklist

- [ ] I know what a MAC Address is.
- [ ] I know why MAC Addresses are important.
- [ ] I know the difference between a MAC Address and an IP Address.
- [ ] I can find my MAC Address on Windows.
- [ ] I can find my MAC Address on Linux.
- [ ] I understand what MAC Address Spoofing is.

---

# 📍 2. Ports and Protocols

## 🤔 What is a Port?

Imagine a large apartment building.

The building has one main address, but inside it there are many apartment numbers.

When a delivery person arrives, the building address tells them where to go, and the apartment number tells them **which apartment** should receive the package.

Networking works in a similar way.

- The **IP Address** identifies the device.
- The **Port Number** identifies the application or service running on that device.

For example:

- Your computer has an IP Address.
- Google Chrome, Discord, Steam, and WhatsApp all use different ports to communicate.

Without ports, your computer would not know which application should receive the incoming data.

---

## ❓ Why Do We Need Ports?

Ports allow multiple applications to use the network at the same time.

For example, you can:

- Watch YouTube.
- Download a file.
- Play an online game.
- Chat on Discord.

All at the same time.

Ports help the operating system send the incoming data to the correct application.

---

## 🌍 Real-Life Example

Think of a hotel.

```
Hotel Address = IP Address

Room Number = Port Number
```

The courier knows the hotel.

But without the room number,

they won't know which guest should receive the package.

Similarly,

without a port number,

the computer won't know which application should receive the network traffic.

---

## 📌 What is a Protocol?

A **Protocol** is a set of rules that devices follow to communicate with each other.

Just like people use a common language to understand each other,

computers use protocols.

Examples include:

- HTTP
- HTTPS
- FTP
- DNS
- SSH
- SMTP

Each protocol has a different purpose, and many of them use well-known port numbers.


---

# 🔄 TCP vs UDP

When devices communicate over a network, they mainly use **two Transport Layer protocols**:

- TCP (Transmission Control Protocol)
- UDP (User Datagram Protocol)

Both are used to send data, but they work differently.

---

## 📌 TCP (Transmission Control Protocol)

TCP is a **reliable** communication protocol.

Before sending data, TCP creates a connection between the sender and the receiver.

It checks if the data reaches the destination correctly.

If any data is lost, TCP sends it again.

Think of TCP like sending an important document through a courier service.

You receive a confirmation when it is delivered.

---

### 🌍 Real-Life Example

Imagine you transfer ₹10,000 using online banking.

You cannot afford to lose even ₹1.

TCP makes sure all the data reaches safely.

---

### Where TCP is Used

- Web Browsing (HTTP/HTTPS)
- Online Banking
- Email
- File Downloads
- SSH

---

### Advantages of TCP

- Reliable
- Error Checking
- Data arrives in the correct order
- Lost packets are retransmitted

---

### Disadvantages of TCP

- Slightly slower
- Uses more resources

---

# 📌 UDP (User Datagram Protocol)

UDP is a **fast** communication protocol.

It sends data without checking whether it reached the destination.

It does not create a connection before sending data.

Think of UDP like making an announcement over a loudspeaker.

You speak once.

Whether everyone hears it or not isn't checked.

---

### 🌍 Real-Life Example

Suppose you're watching a live cricket match.

If one video frame is lost,

the video continues playing.

You don't want the stream to pause every second waiting for missing packets.

That's why streaming services often use UDP.

---

### Where UDP is Used

- Online Games
- Video Calls
- Voice Calls
- Live Streaming
- DNS

---

### Advantages of UDP

- Faster
- Low Delay
- Uses fewer resources

---

### Disadvantages of UDP

- No error checking
- Lost packets are not recovered
- Data may arrive out of order

---

# 📊 TCP vs UDP

| TCP | UDP |
|------|------|
| Reliable | Fast |
| Connection-Oriented | Connectionless |
| Error Checking | No Error Checking |
| Retransmits Lost Data | Doesn't Retransmit |
| Slower | Faster |
| Used for Banking, Email, Downloads | Used for Gaming, Streaming, VoIP |

---

# 📌 Port Number Ranges

Ports range from **0 to 65535**.

They are divided into three categories.

| Range | Name | Purpose |
|--------|------|---------|
| 0 - 1023 | Well-Known Ports | Common services like HTTP, HTTPS, SSH |
| 1024 - 49151 | Registered Ports | Applications and software |
| 49152 - 65535 | Dynamic / Private Ports | Temporary client connections |

---

# 🌐 Common Ports and Protocols

These are some of the most important ports that every cybersecurity beginner should know.

---

## Port 20

### Protocol

FTP (File Transfer Protocol - Data)

### Purpose

Transfers file data between computers.

### Example

Downloading files from an FTP server.

---

## Port 21

### Protocol

FTP (Control)

### Purpose

Controls FTP connections.

### Example

Logging into an FTP Server.

---

## Port 22

### Protocol

SSH (Secure Shell)

### Purpose

Securely access another computer remotely.

### Example

Connecting to a Linux server.

```bash
ssh user@192.168.1.10
```

---

## Port 23

### Protocol

Telnet

### Purpose

Remote access to another computer.

### Note

Telnet is **not secure** because it sends data in plain text.

SSH is preferred today.

---

## Port 25

### Protocol

SMTP (Simple Mail Transfer Protocol)

### Purpose

Sends emails.

### Example

Sending an email from Gmail.

---

## Port 53

### Protocol

DNS (Domain Name System)

### Purpose

Converts domain names into IP addresses.

### Example

```
google.com

↓

142.xxx.xxx.xxx
```

---

## Port 67

### Protocol

DHCP Server

### Purpose

Assigns IP Addresses to devices.

---

## Port 68

### Protocol

DHCP Client

### Purpose

Receives IP Addresses from the DHCP Server.

---

## Port 69

### Protocol

TFTP (Trivial File Transfer Protocol)

### Purpose

Transfers files without authentication.

Mostly used in network devices.

---

## Port 80

### Protocol

HTTP

### Purpose

Loads websites without encryption.

### Example

```
http://example.com
```

---

## Port 110

### Protocol

POP3

### Purpose

Receives emails from the mail server.

---

## Port 123

### Protocol

NTP (Network Time Protocol)

### Purpose

Synchronizes the system time.

---

## Port 143

### Protocol

IMAP

### Purpose

Reads emails while keeping them stored on the mail server.

---

## Port 161

### Protocol

SNMP

### Purpose

Monitors routers, switches, printers, and network devices.

---

## Port 389

### Protocol

LDAP

### Purpose

Directory Services and Active Directory communication.

---

## Port 443

### Protocol

HTTPS

### Purpose

Loads encrypted websites.

### Example

```
https://google.com
```

This is one of the most commonly used ports on the Internet.

---

## Port 445

### Protocol

SMB (Server Message Block)

### Purpose

File and printer sharing in Windows.

---

## Port 3306

### Protocol

MySQL

### Purpose

Database communication.

---

## Port 3389

### Protocol

RDP (Remote Desktop Protocol)

### Purpose

Remote access to Windows computers.

---

## Port 8080

### Protocol

Alternative HTTP

### Purpose

Often used by web applications and development servers.

---

# 📋 Important Ports Cheat Sheet

| Port | Protocol | Purpose |
|------:|----------|---------|
| 20 | FTP (Data) | File Transfer |
| 21 | FTP | FTP Login |
| 22 | SSH | Secure Remote Login |
| 23 | Telnet | Remote Login (Insecure) |
| 25 | SMTP | Send Email |
| 53 | DNS | Domain Name Resolution |
| 67 | DHCP Server | Assign IP Address |
| 68 | DHCP Client | Receive IP Address |
| 69 | TFTP | Simple File Transfer |
| 80 | HTTP | Website |
| 110 | POP3 | Receive Email |
| 123 | NTP | Time Synchronization |
| 143 | IMAP | Email Access |
| 161 | SNMP | Network Monitoring |
| 389 | LDAP | Directory Services |
| 443 | HTTPS | Secure Website |
| 445 | SMB | File Sharing |
| 3306 | MySQL | Database |
| 3389 | RDP | Remote Desktop |
| 8080 | HTTP Alternate | Web Applications |

---

# 🔐 Cybersecurity Importance

### 👨‍💻 SOC Analyst

A SOC Analyst monitors:

- Unusual port activity.
- Suspicious network connections.
- Blocked or unauthorized ports.
- Malicious traffic.

---

### 🛡 Penetration Tester

A Penetration Tester identifies:

- Open ports.
- Running services.
- Misconfigured servers.
- Vulnerable protocols.

---

### 🐞 Bug Bounty Hunter

A Bug Bounty Hunter often checks:

- Open web services.
- Exposed admin panels.
- APIs running on uncommon ports.
- Misconfigured web servers.

---

# 📝 Quick Notes

- A Port identifies an application or service.
- A Protocol defines the rules for communication.
- TCP is reliable.
- UDP is faster.
- Port 80 = HTTP.
- Port 443 = HTTPS.
- Port 22 = SSH.
- Port 53 = DNS.

---

# 💡 Interview Questions

### Q1. What is a Port?

A Port is a logical communication endpoint used by applications to send and receive network data.

---

### Q2. What is a Protocol?

A Protocol is a set of rules that devices follow to communicate over a network.

---

### Q3. Which protocol is more reliable, TCP or UDP?

TCP.

---

### Q4. Which protocol is faster?

UDP.

---

### Q5. Which port is used by HTTPS?

Port 443.

---

### Q6. Which port is used by SSH?

Port 22.

---

### Q7. Which port is used by DNS?

Port 53.

---

# 🎯 Mini Activity

1. Memorize the following ports:

- 22 (SSH)
- 53 (DNS)
- 80 (HTTP)
- 443 (HTTPS)
- 445 (SMB)
- 3389 (RDP)

2. Search your own computer for open ports later when you learn **Nmap**.

---

# ✅ Checklist

- [ ] I know what a Port is.
- [ ] I know what a Protocol is.
- [ ] I understand TCP and UDP.
- [ ] I know the difference between TCP and UDP.
- [ ] I can identify common ports.
- [ ] I know why ports are important in cybersecurity.

---

# 📍 3. DNS (Domain Name System)

## 🤔 What is DNS?

The **Domain Name System (DNS)** is often called the **phonebook of the Internet**.

Humans prefer to remember names like:

```
google.com
```

Computers communicate using IP addresses like:

```
142.250.183.206
```

DNS converts a domain name into its IP address so your computer knows where to connect.

---




