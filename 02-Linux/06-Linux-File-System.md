# 📖 6. Linux File System

> "Everything in Linux is treated as a file."

---

# 🎯 Learning Objectives

After completing this topic, you will be able to:

- Understand what a File System is.
- Understand the Linux directory structure.
- Know the purpose of important Linux directories.
- Navigate the Linux file system with confidence.

---

# 🤔 What is a File System?

A **File System** is the way an operating system stores, organizes, and manages files and folders.

Think of it like a **library**.

📚 A library contains books arranged into different sections.

Similarly,

💻 A computer stores files in different folders so they can be easily found and managed.

Without a file system, your computer wouldn't know where your files are stored.

---

# ❓ Why Do We Need a File System?

A file system helps the operating system to:

- Store files
- Organize folders
- Find files quickly
- Protect files
- Manage storage efficiently

Without it, your computer would be like a room where everything is thrown on the floor.

---

# 🌍 Real-Life Example

Imagine your house.

🏠 House

↓

🚪 Rooms

↓

📦 Cupboards

↓

📁 Drawers

↓

📄 Documents

Linux works the same way.

The entire computer starts from one main folder called **Root (/)**.

Inside it are different folders, each with a specific purpose.

---

# 🌳 Linux Directory Structure

```
                /
                │
 ├── bin
 ├── boot
 ├── dev
 ├── etc
 ├── home
 ├── lib
 ├── media
 ├── mnt
 ├── opt
 ├── proc
 ├── root
 ├── run
 ├── sbin
 ├── srv
 ├── sys
 ├── tmp
 ├── usr
 └── var
```

Everything in Linux starts from **/**

This is called the **Root Directory**.

---

# 📂 Important Linux Directories

---

## 📁 /

### Root Directory

This is the top-level directory.

Everything starts here.

Think of it as the **main entrance** of your house.

---

## 🏠 /home

Stores personal files of users.

Example:

```
/home/ankush
```

Contains:

- Documents
- Downloads
- Pictures
- Music
- Videos

This is where you'll spend most of your time.

---

## 👑 /root

Home directory of the **root (administrator)** user.

Normal users cannot modify it without permission.

Example:

```
/root
```

---

## ⚙️ /etc

Stores configuration files.

Think of it as the **Settings Folder** of Linux.

Examples:

- User settings
- Network configuration
- Password configuration

Cybersecurity professionals often inspect this directory.

---

## 💾 /boot

Contains files required to start (boot) Linux.

Without this folder, Linux cannot start properly.

---

## 📦 /bin

Contains basic commands used by all users.

Examples:

- ls
- cp
- mv
- mkdir

These commands are available immediately after booting.

---

## 🔧 /sbin

Contains important system administration commands.

Examples:

- reboot
- shutdown
- fsck

Mostly used by administrators.

---

## 📚 /usr

Contains applications, software, and libraries installed on the system.

Think of it as the **Program Files** folder in Windows.

---

## 🗂 /var

Stores files that change frequently.

Examples:

- Logs
- Cache
- Mail
- Database files

SOC Analysts often inspect:

```
/var/log
```

because it contains system logs.

---

## 🗑 /tmp

Stores temporary files.

These files are usually deleted after restarting the computer.

Applications use this folder to store temporary data.

---

## 💿 /media

Used when USB drives, CDs, or external storage devices are connected.

Example:

```
/media/USB
```

---

## 📂 /mnt

Used to manually mount storage devices or network drives.

Mostly used by system administrators.

---

## ⚙️ /dev

Contains device files.

Examples:

- Hard Disk
- Keyboard
- Mouse
- USB Drive

Linux treats hardware devices like files.

---

## 🧠 /proc

Contains information about running processes and the system.

This directory is created automatically while Linux is running.

Useful for troubleshooting.

---

## ⚡ /run

Stores temporary information about currently running services.

The data is cleared after reboot.

---

## 🛠 /opt

Used for installing optional or third-party software.

Example:

Some applications install themselves inside:

```
/opt
```

---

## 🌐 /srv

Stores data used by services like:

- FTP
- Web Servers
- File Servers

---

## ⚡ /sys

Contains information about hardware and the Linux Kernel.

Used mainly by advanced users and system administrators.

---

# 📝 Easy Way to Remember

| Folder | Purpose |
|---------|----------|
| / | Starting point of Linux |
| /home | User files |
| /root | Administrator files |
| /etc | Settings & Configuration |
| /boot | Boot files |
| /bin | Basic commands |
| /sbin | Admin commands |
| /usr | Installed programs |
| /var | Logs & changing files |
| /tmp | Temporary files |
| /media | USB drives |
| /mnt | Mounted drives |
| /dev | Hardware devices |
| /proc | Running processes |
| /run | Running services |
| /opt | Optional software |
| /srv | Service data |
| /sys | Kernel & hardware information |

---

# 💡 Why Should a Cybersecurity Professional Learn This?

Understanding the Linux file system helps you:

✅ Find log files

✅ Analyze malware

✅ Investigate incidents

✅ Troubleshoot servers

✅ Perform penetration testing

For example,

If a SOC Analyst wants to investigate suspicious activity,

they'll often check:

```
/var/log
```

If a penetration tester wants to inspect configuration files,

they'll often check:

```
/etc
```

Knowing where to look saves time.

---

# 📝 Quick Notes

✔ Everything starts from `/`.

✔ Linux uses a tree-like directory structure.

✔ `/home` stores user files.

✔ `/etc` stores configuration files.

✔ `/var/log` stores system logs.

✔ `/tmp` stores temporary files.

✔ `/usr` stores installed programs.

✔ `/dev` represents hardware devices.

---

# 💡 Interview Questions

### Q1. What is the Linux Root Directory?

The Root Directory (`/`) is the top-most directory from which all other directories originate.

---

### Q2. Which directory stores user files?

`/home`

---

### Q3. Which directory stores configuration files?

`/etc`

---

### Q4. Where are system logs usually stored?

`/var/log`

---

### Q5. Which directory stores temporary files?

`/tmp`

---

### Q6. Which directory contains installed programs?

`/usr`

---

### Q7. What is the purpose of `/boot`?

It stores files required to start the Linux operating system.

---

# 🎯 Mini Activity

Open your Linux terminal and explore these directories:

```
/
```

```
/home
```

```
/etc
```

```
/var
```

```
/tmp
```

Write down what you observe in each folder.

---

# 📚 Free Resources

### 🎓 Free Courses

- Linux Journey (Filesystem Section)
- Cisco Skills for All - Linux Essentials
- Red Hat Enable Sysadmin Articles

### 🧪 Practice Labs

- TryHackMe – Linux Fundamentals Part 1
- OverTheWire – Bandit
- Hack The Box Academy – Linux Fundamentals

---

# ✅ Checklist

- [ ] I know what a File System is.
- [ ] I know what the Root Directory (`/`) is.
- [ ] I know the purpose of `/home`.
- [ ] I know the purpose of `/etc`.
- [ ] I know the purpose of `/var`.
- [ ] I know the purpose of `/tmp`.
- [ ] I know why understanding the Linux file system is important in cybersecurity.
