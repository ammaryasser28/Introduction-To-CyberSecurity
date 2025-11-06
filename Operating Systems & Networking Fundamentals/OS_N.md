# Operating Systems & Networking Fundamentals

---

## 1) Operating System (OS)

The Operating System is the core software that manages hardware components and provides a platform for applications to run.  
It acts as a bridge between the user, applications, and the hardware.

**Examples:** Windows, Linux, macOS, Android, iOS

---

## 2) OS as a Resource Manager

The OS manages and allocates system resources such as:
- CPU (processing time)
- RAM (memory usage)
- Storage (file systems)
- Input/Output devices (keyboard, printer, network card)

It ensures that programs run efficiently without interfering with each other.

---

## 3) OS as an Interface Provider

The OS provides user interfaces that allow interaction with the system:
- **GUI (Graphical User Interface):** e.g., Windows desktop
- **CLI (Command Line Interface):** e.g., Linux terminal

This makes it easier for users and applications to communicate with the hardware.

---

## 4) OS as a System Coordinator

The OS coordinates and controls how software and hardware interact.  
It ensures operations happen in an organized manner (e.g., reading a file, sending data over the network, running applications).

---

## 5) Kernel

The Kernel is the core component of the OS.  
It operates at the lowest level and communicates directly with the hardware.

**Main responsibilities:**
- Process management
- Memory management
- File system control
- Device control and drivers
- System security and permissions

---

## 6) Types of Operating Systems

| Type | Description | Example |
|------|-------------|---------|
| Single-User | Designed for one user at a time | Windows 10 |
| Multi-User | Supports multiple users simultaneously | Linux Server |
| Desktop OS | For personal computing | Windows, macOS |
| Server OS | Designed to provide services over networks | Ubuntu Server, Windows Server |
| Real-Time OS (RTOS) | Responds quickly to real-time tasks | Aircraft systems, robotics |

---

## 7) HDD vs RAM

| Feature | HDD / SSD | RAM |
|--------|-----------|-----|
| Purpose | Long-term storage | Temporary memory for running applications |
| Speed | HDD (slow) / SSD (fast) | Very fast |
| Data Retention | Keeps data after shutdown | Data is lost when powered off |
| Impact | Affects boot and load times | Affects overall system responsiveness and multitasking |

---

## 8) Networking

Networking involves connecting computers and devices to share data and resources.

**Purposes:**
- Data communication
- Resource sharing (printers, files)
- Internet access

---

## 9) LAN vs WAN

| Network | Coverage | Example | Speed |
|--------|----------|---------|-------|
| **LAN (Local Area Network)** | Small geographic area (home, office) | Home Wi-Fi / Company network | Fast |
| **WAN (Wide Area Network)** | Large geographic area (cities, countries) | The Internet | Slower |

---

## 10) Router vs Switch

| Device | Function | Layer | Use Case |
|-------|----------|-------|---------|
| **Switch** | Connects devices within the same LAN | Layer 2 (Data Link) | Connects PCs inside a network |
| **Router** | Connects different networks together | Layer 3 (Network) | Connects LAN to the Internet |

---

## 11) ARP Protocol (Address Resolution Protocol)

ARP is used to map an **IP Address** to a **MAC Address** within a local network (LAN).  
It allows devices to find each other physically on the same network.

---

## 12) Packets

In networking, data is divided into small units called **packets** before being transmitted.  
Each packet contains:
- Source IP
- Destination IP
- Data being transferred
- Additional routing and control information

Breaking data into packets increases speed, efficiency, and reliability.

---

