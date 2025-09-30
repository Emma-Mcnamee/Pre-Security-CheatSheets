# DHCP (Dynamic Host Configuration Protocol) Cheatsheet
**Topic:** DHCP in Networking  
**Purpose:** Quick reference for understanding how IP addresses are assigned dynamically on a network.

---

## What is DHCP?
**DHCP (Dynamic Host Configuration Protocol)** automatically assigns IP addresses and network configuration to devices on a network.  
- Avoids manual IP assignment.  
- Ensures unique IP addresses and reduces configuration errors.

---

## How DHCP Works
When a device joins a network without an IP address, it follows the **DORA process**:

1. **DHCP Discover:**  
   - Device broadcasts a request to find available DHCP servers on the network.

2. **DHCP Offer:**  
   - The DHCP server responds with an available IP address and network configuration that the device can use.

3. **DHCP Request:**  
   - The device replies to the DHCP server, indicating it wants to use the offered IP address.

4. **DHCP Acknowledgment (ACK):**  
   - The DHCP server confirms the IP assignment and the device can now use the IP to communicate on the network.

---

## Key Points
- DHCP automates IP address assignment.  
- The process ensures each device has a **unique IP**, **subnet mask**, **gateway**, and optionally **DNS server addresses**.  
- Reduces administrative overhead in large networks.  

---

## Quick Diagram of DORA Process
```text
Device                        DHCP Server
  |         DHCP Discover      |
  |---------------------------->|
  |         DHCP Offer          |
  |<----------------------------|
  |         DHCP Request        |
  |---------------------------->|
  |         DHCP ACK            |
  |<----------------------------|
Device now has an IP address
