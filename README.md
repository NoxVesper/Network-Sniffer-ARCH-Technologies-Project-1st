# 🕵️‍♂️ Basic Network Sniffer

**By Rashid Iqbal | AI Red Teamer 🛡️**  
**Cyber Internship Project at ARCH Technologies**

A Python-based **Network Packet Sniffer** to capture and analyze live network traffic on Linux interfaces (e.g., eth0, wlan0) using raw sockets. This project was completed as a practical lab and documented by me to demonstrate real-time packet analysis and network layer understanding.  

---

## 🎯 Objective

The main goals of this project were to:

1. Capture live network traffic using Python 🐍  
2. Understand the structure of network packets at different layers: **Ethernet, IP, TCP/UDP/ICMP** 🌐  
3. Display packet details in a readable format to study how computers communicate over a network 💻  

---

## 🧠 Key Concepts Learned

### Ethernet Frame
- Every packet starts with an Ethernet frame, like the “envelope” of the message ✉️  
- Contains:  
  - **Destination MAC:** The device the packet is for  
  - **Source MAC:** The device sending the packet  
  - **Protocol Type:** Identifies the carried protocol (IPv4, ARP, etc.)  
- Helped me understand the **first layer of network communication**.

### IPv4 Packet
- Main structure for sending data over the internet 🌍  
- Contains:  
  - **Version & Header Length**  
  - **TTL (Time To Live)**  
  - **Protocol**  
  - **Source & Destination IP addresses**  
- Taught me how computers **identify each other and route information**.

### TCP Segment
- Connection-based protocol 🔗  
- Contains:  
  - **Source & Destination Ports** (identify applications/services like HTTP/SSH)  
  - **Sequence & Acknowledgment Numbers** (manage reliable delivery)  
  - **Flags (SYN, ACK, FIN, etc.)** (control connection setup/termination)  
- Helped me track how **connections start, maintain, and end**.

### UDP Segment
- Connectionless protocol ⚡  
- Contains:  
  - **Source & Destination Ports**  
  - **Length of data**  
- Faster than TCP, used for **DNS queries, streaming, etc.**  
- Helped me learn the difference between **reliable and fast protocols**.

### ICMP Packet
- Used for **network diagnostics** (like ping) 🖧  
- Contains:  
  - **Type & Code** (echo request/reply, etc.)  
  - **Checksum** (ensures data integrity)  
- Taught me how **network troubleshooting messages** work.

### Raw Data & Hexadecimal Representation
- Unknown or unsupported protocols are displayed as **raw hexadecimal** 🔢  
- Shows actual bytes being sent, useful for analyzing unusual or custom protocols.

---

## 🐍 Python Implementation

- Used **Python raw sockets** to capture packets.  
- Functions created to:  
  - Parse **Ethernet frames**  
  - Parse **IPv4 headers**  
  - Extract **TCP, UDP, and ICMP data**  
  - Format output neatly for readability  
- Showed how Python can **interact directly with network interfaces**.

---

## 💡 Practical Use

This sniffer helps me:  
- Learn **network communication in real-time** ⏱️  
- Understand **packet structures** 🧩  
- Detect **unusual or suspicious activity** ⚠️  
- Debug and analyze **network traffic** 🖥️  

Essentially, it visualizes the **invisible “conversations” between devices**.

---

## ✅ Conclusion

Exploring the hidden world of network traffic taught me valuable skills and insights:  
- Built a Packet Sniffer to monitor and analyze network traffic 📊  
- Gained hands-on experience with **network layers, protocols, and packet structures**  
- Learned to **capture, parse, and interpret live network data** using Python  
- Developed a deeper understanding of **device communication over a network**  
- Strengthened my knowledge in **Networking, Cybersecurity, and Ethical Hacking** 🛡️  
- Prepared for **real-world tasks in network analysis and security testing**  

---

## 👨‍💻 Author

**Name:** Rashid Iqbal  
**GitHub:** (https://github.com/NoxVesper)  
**📧 Email:** echoinject@gmail.com  

Suggestions for **improvements or bug reports** are highly appreciated! 📝  

---

⚠️ **Disclaimer:** Everything here is for **educational and ethical purposes**. I only hunt where I am invited.
