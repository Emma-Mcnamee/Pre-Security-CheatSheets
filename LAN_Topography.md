# LAN Topologies Cheatsheet
**Topic:** LAN (Local Area Network) Topography  
**Purpose:** Quick reference for network design, topologies, and hardware components  

---

## What is a LAN?
A **Local Area Network (LAN)** is a network that connects devices within a limited area, such as an office, building, or campus.  
**LAN Topography** refers to the design or layout of the network—how devices are connected and how data flows.

---

## LAN Topologies

### 1. Star Topology
- **Design:** All devices connect to a central hub or switch via individual cables.
- **Pros:**  
  - Highly scalable  
  - Reliable—issues on one device do not affect others  
- **Cons:**  
  - Expensive due to cabling and hardware requirements  
  - If the central hub/switch fails, the entire network goes down (though robust devices mitigate this)  
- **Use Case:** Common in modern networks where reliability and scalability are priorities.

---

### 2. Bus Topology
- **Design:** All devices connect along a single backbone cable.
- **Pros:**  
  - Simple setup with minimal cabling  
- **Cons:**  
  - Prone to bottlenecks as all data travels the same path  
  - Troubleshooting is difficult  
  - Minimal redundancy—failure of the backbone affects the whole network  
- **Use Case:** Small networks where cost savings are important and high performance is not critical.

---

### 3. Ring Topology
- **Design:** Devices connect to each other in a circular loop, passing data sequentially.
- **Pros:**  
  - Easy to troubleshoot because data flows in a single direction  
  - Less bottlenecking than bus topology  
- **Cons:**  
  - If any connection is cut, the entire network fails  
  - Devices can only send data after passing along data from previous devices  
- **Use Case:** Networks requiring orderly data transmission; less common today due to vulnerability to single points of failure.

---

## Key Hardware Components

### Switch
- Central device that devices plug into to communicate with each other.  
- Sends data packets to the correct destination within the network.  
- Connecting a **switch to a router** increases redundancy and access to external networks.  
- **Data flow example:** `Device -> Switch -> Router -> Internet`

### Router
- Connects multiple networks and directs data between them.  
- Handles **routing**, which is the process of deciding how data travels between networks.  
- Essential for connecting LANs to WANs (e.g., Internet).

---

## Quick Comparison Table

| Topology | Pros | Cons | Use Case |
|----------|------|------|---------|
| Star     | Scalable, reliable | Expensive, central point of failure | Modern office networks |
| Bus      | Simple, cheap | Bottlenecks, hard to troubleshoot, low redundancy | Small networks |
| Ring     | Easy troubleshooting, less bottleneck | Single failure cuts network | Orderly data transmission networks |

---

## Tips for Remembering
- **Star** = all paths lead to the center. Think of a star in the sky.  
- **Bus** = a single road everyone travels on. Traffic jams (bottlenecks) happen easily.  
- **Ring** = circular track; data goes one direction around the loop.  

---

This file can serve as a quick reference or cheat sheet for interviews, exams, or hands-on labs.
