# Subnetting Cheatsheet
**Topic:** Subnetting in Networking  
**Purpose:** Quick reference for understanding subnetting, IP usage, and network addresses.

---

## What is Subnetting?
**Subnetting** is the process of splitting a large network into smaller, manageable sub-networks (subnets).  
- Helps organize network devices into groups based on function or department.  
- Provides **efficiency**, **security**, and **better control** of network traffic.  

**Example:**  
A company network may be split into:  
- Accounting subnet  
- Finance subnet  
- HR subnet  

---

## Key Concepts

### 1. Subnet Mask
- Defines the range of IP addresses within a subnet.  
- Helps devices determine which IP addresses belong to the local subnet vs. external networks.

### 2. IP Address Uses in Subnets
Subnets use IP addresses in three main ways:  
1. **Host Address** – The IP assigned to a device within the subnet.  
2. **Network Address** – Identifies the subnet itself.  
3. **Default Gateway Address** – The “door” to external networks, used when sending data outside the subnet.  

---

## Definitions

- **Host Address:** The unique IP assigned to a device (computer, printer, server) within a subnet.  
- **Network Address:** Represents the subnet as a whole; used to identify the network.  
- **Default Gateway:** The IP address of the router that devices use to send traffic outside their subnet.  
  - Think of it as the “door” to the Internet or other networks.  

---

## Benefits of Subnetting
- **Efficiency:** Reduces unnecessary traffic by limiting broadcasts to smaller networks.  
- **Security:** Separates departments or functions to control access.  
- **Control:** Makes IP management and troubleshooting easier for network admins.  

---

## Quick Example

| Subnet | Host IP Range | Network Address | Default Gateway |
|--------|---------------|----------------|----------------|
| Accounting | 192.168.1.1–192.168.1.50 | 192.168.1.0 | 192.168.1.254 |
| Finance    | 192.168.2.1–192.168.2.50 | 192.168.2.0 | 192.168.2.254 |
| HR         | 192.168.3.1–192.168.3.50 | 192.168.3.0 | 192.168.3.254 |

---

## Tips
- Always know the **network address** and **default gateway** for troubleshooting connectivity.  
- Subnetting allows for **logical separation** of departments without additional hardware.  
- Use subnet masks to calculate host ranges and identify available IPs per subnet.  

---

This cheatsheet can be used for quick reference in labs, interviews, or GitHub repos.
