# Cisco Packet Tracer – Basic Router Interface Configuration

## Overview

This Packet Tracer lab demonstrates the basic configuration of a Cisco router connecting three different LANs.

The exercise includes:

- Configuring the router hostname
- Assigning IPv4 addresses to router interfaces
- Enabling router interfaces
- Adding interface descriptions
- Configuring PCs with static IP addresses
- Saving the router configuration
- Testing end-to-end connectivity using ping

---

## Network Topology

<img width="784" height="297" alt="image" src="https://github.com/user-attachments/assets/b7fcfb19-64ee-4ac3-a4a9-1dcd79d7fbf2" />


---

## IP Addressing Table

| Device | Interface | IP Address | Subnet Mask |
|---------|-----------|------------|-------------|
| R1 | G0/0 | 15.255.255.254 | 255.0.0.0 |
| R1 | G0/1 | 182.98.255.254 | 255.255.0.0 |
| R1 | G0/2 | 201.191.20.254 | 255.255.255.0 |
| PC1 | FastEthernet0 | 15.0.0.1 | 255.0.0.0 |
| PC2 | FastEthernet0 | 182.98.0.1 | 255.255.0.0 |
| PC3 | FastEthernet0 | 201.191.20.1 | 255.255.255.0 |

---

## Objectives

- Configure the router hostname.
- Configure router interfaces.
- Assign IPv4 addresses.
- Enable interfaces.
- Add interface descriptions.
- Configure PCs with static IP addresses.
- Verify interface status.
- Save the running configuration.
- Test connectivity using ping.

---

# Step 1 – Configure Router Interfaces

Configured the following interfaces:

- GigabitEthernet0/0
- GigabitEthernet0/1
- GigabitEthernet0/2

Each interface was assigned the correct IP address, description, and enabled using the **no shutdown** command.


## Router Configuration
<img width="952" height="464" alt="configuring_router_interfaces" src="https://github.com/user-attachments/assets/f8a31629-ae39-4060-b282-261b1da30a57" />



---

# Step 2 – Verify Router Interfaces

Verified the configuration using:

```text
show ip interface brief
```

Output confirmed:

- Interfaces are UP
- Protocol status is UP
- Correct IP addresses assigned

---

## Interface Verification

<img width="440" height="68" alt="confirming_interface_configuration" src="https://github.com/user-attachments/assets/ac0e938f-6696-4284-9c2c-7b06c42c47e7" />


---

# Step 3 – Configure PC1

Configured:

IP Address:

```
15.0.0.1
```

Subnet Mask

```
255.0.0.0
```

Default Gateway

```
15.255.255.254
```

<img width="951" height="463" alt="configuring_PC-1&#39;s ip address" src="https://github.com/user-attachments/assets/d4be2494-62c0-4576-8da8-fa41b6715a8f" />

---

# Step 4 – Configure PC2

Configured:

IP Address

```
182.98.0.1
```

Subnet Mask

```
255.255.0.0
```

Default Gateway

```
182.98.255.254
```

<img width="952" height="467" alt="configuring_PC-2_ip address" src="https://github.com/user-attachments/assets/be136e6b-5f24-45b2-9c0f-20be12fc4adb" />


---

# Step 5 – Configure PC3

Configured:

IP Address

```
201.191.20.1
```

Subnet Mask

```
255.255.255.0
```

Default Gateway

```
201.191.20.254
```


<img width="954" height="469" alt="configuring_PC-3&#39;s ip address" src="https://github.com/user-attachments/assets/30c33199-164a-4eff-b3cf-1722b4567902" />


---

# Step 6 – Connectivity Test

Connectivity was verified using the **ping** command from PC1.

Successful communication was established with:

- PC2
- PC3

The first ping request timed out because the ARP table had not yet been populated. Subsequent replies were successful, confirming proper routing.

<img width="952" height="485" alt="confirming_i_can_reach_pc2 and pc3 from pc1" src="https://github.com/user-attachments/assets/2e7a9fdc-10c2-4415-930c-e18b3b678818" />


---

# Skills Demonstrated

- Cisco IOS CLI
- Router configuration
- Interface configuration
- IPv4 addressing
- Static IP configuration
- Interface descriptions
- Cisco Packet Tracer
- Basic routing
- Connectivity testing
- Network troubleshooting

---

# Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4
- Ethernet Networking

---

# Author

**Susan Wangari**

Bachelor of Science in Mathematics and Computer Science

Networking | Cybersecurity | Cisco CCNA
