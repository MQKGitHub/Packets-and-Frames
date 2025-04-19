## 🛡️ Packets & Frames

**Room:** [Packets & Frames — TryHackMe]((https://tryhackme.com/room/packetsframes))
**Status:** ✅ Completed  
**Date:** *(19 April 2025)*

### 🎯 Objective
To learn how data is transmitted across networks using packets and frames, understand how the TCP/IP model works (including the three-way handshake), compare TCP and UDP protocols, and explore the use of ports and common network services.

---

### 🗝️ Key Concepts  
- **Packets and Frames** – Small chunks of data used to send information across a network. Packets work at Layer 3, frames at Layer 2.  
- **Encapsulation** – The process of wrapping data with extra information as it moves through the network layers.  
- **Packet Headers** – Extra data in a packet that includes things like source/destination IPs, TTL, and error checking with checksums.  
- **TCP Protocol** – A connection-based protocol that ensures data arrives in order and without errors using a three-way handshake.  
- **Three-Way Handshake** – The process of setting up a TCP connection using SYN, SYN/ACK, and ACK messages.  
- **Sequence and Acknowledgement Numbers** – Used by TCP to keep track of which pieces of data have been sent and received.  
- **TCP Connection Closure** – A clean way to end a connection using FIN and ACK messages to release resources.  
- **UDP Protocol** – A faster but less reliable protocol that sends data without confirming delivery, used in things like streaming or voice calls.  
- **Ports** – Numbered access points (0–65535) used to handle different services on a device, like websites, file sharing, or remote login.  
- **Common Port Numbers** – Standard ports for services: 21 (FTP), 22 (SSH), 80 (HTTP), 443 (HTTPS), 445 (SMB), 3389 (RDP).

---

### 🛠️ Tools Used
- TryHackMe Virtual Machine and built-in tools
- Packet analysis tools (not specified, but conceptually relevant)
- Static lab for reconstructing the TCP handshake

---

### ⚠️ Challenges Faced
- Initially confusing the difference between packets and frames, especially which layers they belong to in the OSI model.
- Wrapping my head around how TCP sequences and acknowledgements work with numbers.

---

### 🧠 What I Learned
- Frames are layer 2 (Data Link Layer), while packets are layer 3 (Network Layer).
- TCP is reliable and connection-based; UDP is faster but doesn't guarantee delivery.
- Each TCP/UDP packet contains headers like source/destination IP, ports, sequence numbers, etc.
- The three-way handshake is essential for establishing a TCP connection.
- Ports allow applications to communicate through predefined channels (e.g. HTTP on 80).

---

### 🌐 Real-World Application:
> Understanding TCP/IP is fundamental for any cybersecurity role, especially in penetration testing or network forensics.  
> For example, knowing how to analyse packet headers can help detect spoofed IPs or session hijacking.  
> Also, recognising what services are running on certain ports is vital for scanning and enumeration during assessments.

---

### 💭 Reflections:
- The breakdown of the TCP handshake using Alice and Bob really helped it click — it made the abstract concept easier to follow.
- Learning about ports through real-world protocol examples made it less dry than expected.
- One takeaway I won’t forget is how critical packet structure is in ensuring data integrity and reliable communication on the internet.
