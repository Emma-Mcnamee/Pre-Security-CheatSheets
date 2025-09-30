# OSI Model (Open Systems Interconnection) Cheatsheet
**Topic:** OSI Model in Networking  
**Purpose:** Quick reference for understanding the seven layers, their functions, and protocols.

---

## What is the OSI Model?
The **OSI Model** provides a standardized framework that dictates how networked devices **send, receive, and interpret data**.  
- Ensures devices of different types can communicate seamlessly.  
- **Encapsulation:** At each layer, data is wrapped with relevant information for transmission.

---

## OSI Model Layers

### Layer 1 — Physical
- **Role:** Deals with the physical hardware used in networking.  
- **Data Representation:** Transmits data as electrical signals (binary 1s and 0s).  
- **Examples:** Cables, switches, hubs, NICs.  
- **Notes:** Lowest layer; ensures physical transmission between devices.

---

### Layer 2 — Data Link
- **Role:** Handles **physical addressing** and prepares data for transmission on the physical layer.  
- **Function:** Receives packets from the Network layer and adds the **MAC address** of the destination device.  
- **Examples:** Switches, bridges, network interface cards.  

---

### Layer 3 — Network
- **Role:** Responsible for **routing and reassembly** of data.  
- **Function:** Determines the optimal path for data to reach its destination.  
- **Devices:** Routers are Layer 3 devices.  
- **Protocols:**  
  - IP (Internet Protocol)  
  - OSPF (Open Shortest Path First)  
  - RIP (Routing Information Protocol)  
- **Notes:** Handles IP addresses and logical addressing.

---

### Layer 4 — Transport
- **Role:** Ensures reliable data transmission between devices.  
- **Protocols:**

**1. TCP (Transmission Control Protocol)**  
- Guarantees reliability; maintains a constant connection while data is sent.  
- Performs error checking and ensures data is received in order.  
- Can be slower due to connection management and error correction.  

**2. UDP (User Datagram Protocol)**  
- Connectionless; faster but unreliable.  
- No error checking; allows applications to manage data integrity.  
- Pros: Low latency, high speed.  
- Cons: Data may be lost or arrive out of order.

---

### Layer 5 — Session
- **Role:** Maintains connections between devices.  
- **Function:** Establishes, manages, and terminates sessions.  
- **Notes:** Keeps track of conversations and communication state.

---

### Layer 6 — Presentation
- **Role:** Acts as a translator for data between Application and lower layers.  
- **Function:** Ensures standardization across different applications (e.g., email clients).  
- **Additional:** Handles security, encryption, and HTTPS protocols.

---

### Layer 7 — Application
- **Role:** Determines how users interact with the data.  
- **Function:** Provides interfaces and protocols for end-user applications (e.g., browsers, email clients, file transfer).  

---

## Quick Layer Summary

| Layer | Role / Function | Key Devices / Protocols |
|-------|----------------|------------------------|
| 7 Application | User interface for data | Browsers, FTP clients, email apps |
| 6 Presentation | Data translation & encryption | SSL/TLS, JPEG, MPEG |
| 5 Session | Connection management | NetBIOS, PPTP, SSH |
| 4 Transport | Reliable / fast transmission | TCP, UDP |
| 3 Network | Routing & logical addressing | Routers, IP, OSPF, RIP |
| 2 Data Link | Physical addressing | Switches, MAC, bridges |
| 1 Physical | Hardware & electrical signals | Cables, hubs, NICs |

---

## Tips
- Remember **“Please Do Not Throw Sausage Pizza Away”** for OSI Layer order: Physical → Data Link → Network → Transport → Session → Presentation → Application.  
- **TCP** = reliable, connection-oriented; **UDP** = fast, connectionless.  
- Security features like encryption usually occur at Layer 6.  
- Routers operate at Layer 3; switches at Layer 2.  

---

This cheatsheet is useful for labs, exams, networking certifications, or GitHub repositories.
