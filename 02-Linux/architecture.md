# 📖 5. Linux Architecture

## 🤔 What is Linux Architecture?

Linux Architecture refers to **how the Linux Operating System is organized** and **how different parts work together**.

Think of Linux as a company.

Everyone has a different job, and together they keep everything running smoothly.

Similarly, Linux has different components that work together.

---

# 🏗 Linux Architecture Diagram

                +----------------------+
                |       User           |
                +----------------------+
                          │
                          ▼
                +----------------------+
                |   Applications       |
                | (Chrome, VS Code)    |
                +----------------------+
                          │
                          ▼
                +----------------------+
                |       Shell          |
                |   (Bash / Zsh)       |
                +----------------------+
                          │
                          ▼
                +----------------------+
                |      Kernel          |
                +----------------------+
                          │
                          ▼
                +----------------------+
                |      Hardware        |
                | CPU • RAM • Disk     |
                +----------------------+

---

# 🧑 User

The **User** is the person using the computer.

Examples:

- You
- Me
- A System Administrator
- A Hacker
- A Developer

The user gives commands to the computer.

---

# 💻 Applications

Applications are the programs you use every day.

Examples:

- Google Chrome
- Firefox
- VS Code
- LibreOffice
- VLC
- Burp Suite
- Wireshark

Applications cannot directly communicate with the hardware.

They ask the Operating System to perform tasks.

---

# 💲 Shell

The **Shell** is a program that accepts commands from the user.

It acts as a translator.

It understands your commands and sends them to the Kernel.

Popular Linux Shells:

- Bash (Most Common)
- Zsh
- Fish

Example:

```
ls
```

You type this command.

The Shell sends it to the Kernel.

The Kernel gets the list of files.

The Shell displays the result.

---

# ❤️ Kernel

The **Kernel** is the heart of Linux.

It manages everything inside the computer.

Responsibilities:

- CPU Management
- Memory (RAM)
- Storage
- Processes
- Devices
- Network
- Security

Without the Kernel, Linux cannot work.

---

# 🖥 Hardware

Hardware is the physical part of the computer.

Examples:

- CPU
- RAM
- SSD
- HDD
- Keyboard
- Mouse
- Monitor
- Network Card

The Kernel communicates directly with the hardware.

---

# 🔄 How Linux Works

Let's understand with an example.

Suppose you type:

```
mkdir Cybersecurity
```

Step 1

You type the command.

↓

Step 2

The Shell receives the command.

↓

Step 3

The Shell sends it to the Kernel.

↓

Step 4

The Kernel asks the Hard Disk to create a new folder.

↓

Step 5

The folder is created.

↓

Step 6

The Shell shows the result to you.

Everything happens in just a fraction of a second.

---

# 🌍 Real-Life Example

Imagine ordering food.

👤 You = User

🍽 Waiter = Shell

👨‍🍳 Chef = Kernel

🍳 Kitchen = Hardware

You tell the waiter what you want.

The waiter tells the chef.

The chef prepares the food using the kitchen.

The waiter brings the food back.

Linux works in the same way.

---

# 📝 Quick Notes

✅ User gives commands.

✅ Shell understands commands.

✅ Kernel manages the computer.

✅ Hardware performs the work.

✅ Applications use the Kernel to access hardware.

---

# 💡 Interview Questions

### Q1. What is Linux Architecture?

Linux Architecture is the structure of the Linux Operating System and how its components work together.

---

### Q2. What is a Shell?

A Shell is a command interpreter that accepts user commands and passes them to the Kernel.

---

### Q3. What is the Kernel?

The Kernel is the core part of the Linux Operating System that manages hardware and system resources.

---

### Q4. Can applications directly communicate with hardware?

No.

Applications communicate with the Kernel, and the Kernel communicates with the hardware.

---

### Q5. Name three popular Linux shells.

- Bash
- Zsh
- Fish

---

# 🎯 Mini Activity

Draw the Linux Architecture diagram in your notebook.

Label:

- User
- Applications
- Shell
- Kernel
- Hardware

Understanding this diagram will help you throughout your Linux journey.

---

# ✅ Checklist

- [ ] I know what Linux Architecture is.
- [ ] I know what a Shell does.
- [ ] I know what a Kernel does.
- [ ] I understand how Linux processes commands.
- [ ] I can explain Linux Architecture in simple words.
