# ARP (Address Resolution Protocol) Cheatsheet
**Topic:** ARP in Networking  
**Purpose:** Quick reference for understanding how devices map IP addresses to MAC addresses on a network.

---

## What is ARP?
**ARP (Address Resolution Protocol)** allows devices on a network to identify each other by mapping **IP addresses** to **MAC addresses**.  
- Essential for communication within a local network (LAN).  
- Works at the **Data Link Layer (Layer 2)** and **Network Layer (Layer 3)**.

---

## How ARP Works
1. **ARP Cache:**  
   - Every device maintains a local **cache** (ledger) storing known IP-to-MAC mappings.  
   - Reduces the need to repeatedly request MAC addresses.

2. **ARP Request:**  
   - When a device wants to communicate with another IP on the same network and doesn’t have its MAC in the cache, it broadcasts an **ARP request**.  
   - The request asks: “Who has IP X.X.X.X? Please send your MAC address.”

3. **ARP Reply:**  
   - The device with the requested IP responds with its **MAC address**.  
   - The requester stores this mapping in its ARP cache for future communication.

---

## Key Points
- ARP maps **logical addresses (IP)** to **physical addresses (MAC)**.  
- ARP caches help reduce network traffic and speed up communication.  
- ARP operates **only within a local network**; routers are needed to communicate between subnets.  
- ARP can be viewed or manipulated for troubleshooting using commands like `arp -a`
