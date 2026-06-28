# Cisco Device Basics

## Project Overview

This project demonstrates the initial deployment and secure configuration of Cisco networking devices for a small office environment using Cisco Packet Tracer.

The lab focuses on foundational Cisco IOS configuration tasks required to bring a new network online, including router and switch configuration, IPv4 addressing, secure administrative access, and connectivity verification.

---

## Business Scenario

Campbell Technologies is opening a new office and requires a basic network infrastructure before employees can begin working.

As the network engineer, I was responsible for:

- Deploying a Cisco router and switch
- Configuring device hostnames
- Assigning IPv4 addresses
- Configuring secure administrative access
- Establishing connectivity between network devices
- Verifying network functionality
- Documenting the deployment process

---

## Objectives

- Configure a Cisco router from factory defaults
- Configure a Cisco switch from factory defaults
- Configure management IP addressing
- Configure secure passwords
- Configure SSH remote management
- Verify interface status
- Test Layer 3 connectivity
- Save configurations
- Document the completed deployment

---

## Network Topology

*(Insert your topology screenshot here)*

Example:

![Network Topology](screenshots/01_topology.png)

---

## Equipment

| Device | Model |
|---------|-------|
| Router | Cisco 1941 |
| Switch | Cisco Catalyst 2960 |
| End Device | PC |
| Software | Cisco Packet Tracer |

---

## IP Addressing Plan

| Device | Interface | IP Address | Subnet Mask |
|---------|-----------|------------|-------------|
| R1 | G0/0 | 192.168.10.1 | 255.255.255.0 |
| SW1 | VLAN 1 | 192.168.10.2 | 255.255.255.0 |
| PC1 | NIC | 192.168.10.10 | 255.255.255.0 |

Default Gateway

```
192.168.10.1
```

---

## Technologies Used

- Cisco IOS
- Cisco Packet Tracer
- IPv4
- SSH
- Cisco CLI

---

## Skills Demonstrated

- Cisco router configuration
- Cisco switch configuration
- Interface configuration
- IPv4 addressing
- Secure remote management
- SSH configuration
- Network verification
- Troubleshooting
- Technical documentation

---

## Configuration Tasks Completed

- Configured hostnames
- Configured enable secret
- Configured console access
- Configured MOTD banner
- Disabled DNS lookup
- Configured router interface
- Configured switch management interface
- Configured default gateway
- Enabled SSH
- Generated RSA keys
- Saved startup configuration

---

## Verification

The following commands were used to verify the deployment.

```text
show ip interface brief

show running-config

show startup-config

show version

show inventory

show ip ssh

ping
```

---

## Screenshots

### Network Topology

![Topology](screenshots/01_topology.png)
<img width="104" height="242" alt="image" src="https://github.com/user-attachments/assets/62d73199-305b-40aa-b7c3-a9a8ccf4dc67" />

---

### Router Configuration

![Router](screenshots/02_router_running_config.png)
<img width="185" height="413" alt="image" src="https://github.com/user-attachments/assets/8bad814a-6304-4676-b0f5-bcecd3b44217" />
<img width="151" height="395" alt="image" src="https://github.com/user-attachments/assets/def9a143-4772-42ca-a897-194628de4e41" />
<img width="298" height="41" alt="image" src="https://github.com/user-attachments/assets/4375f9c5-9f2d-4cac-8382-8e281e4fc4ff" />

---

### Switch Configuration

![Switch](screenshots/04_switch_running_config.png)

---

### Successful Connectivity Test

![Ping](screenshots/06_successful_ping.png)

---

## Troubleshooting

### Issue

Router interface remained administratively down.

### Cause

The interface had not been enabled.

### Resolution

Configured:

```text
no shutdown
```

---

### Issue

Unable to ping the router.

### Cause

Incorrect default gateway configured on the PC.

### Resolution

Updated the default gateway to:

```
192.168.10.1
```

---

## Lessons Learned

This project reinforced the importance of following a structured deployment process when configuring Cisco networking devices.

Key takeaways include:

- Secure devices before deployment.
- Verify every configuration step.
- Test connectivity after each change.
- Save configurations to prevent data loss.
- Document all implementation and troubleshooting activities.

---

## Future Improvements

Future versions of this project will include:

- VLAN implementation
- Trunk links
- DHCP
- Access Control Lists (ACLs)
- Port Security
- OSPF routing
- Enterprise network expansion

---

## Author

**Ewan Campbell**

Aspiring Cybersecurity Professional

CompTIA A+ Certified

CompTIA Network+ Certified

Associate of Science in Network Systems Technology (Cybersecurity)
## Project Roadmap

- ✅ Project 1: Cisco Device Basics
- ⬜ Project 2: Small Office LAN
- ⬜ Project 3: VLAN Segmentation
- ⬜ Project 4: DHCP Services
- ⬜ Project 5: Static Routing
- ⬜ Project 6: RIP Routing
- ⬜ Project 7: EIGRP Enterprise Network
- ⬜ Project 8: OSPF Enterprise Network
- ⬜ Project 9: Network Security
- ⬜ Project 10: Business Acquisition (RIP ↔ EIGRP)
- ⬜ Project 11: Campus Network
- ⬜ Project 12: Enterprise Network Capstone
