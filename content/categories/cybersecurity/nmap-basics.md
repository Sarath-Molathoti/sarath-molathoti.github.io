# Nmap in Ethical Hacking | Port Scanning

**Posted on October 21, 2024**

## Tags

- Ethical Hacking
- Nmap
- Port Scanning

---

## What is a Port?

Ports are numerical identifiers for specific network services or applications. Each device or server uses ports to differentiate between different services (like email, web servers, file transfer, etc.). A device can have up to 65,536 ports, divided into:

1. **Well-known ports (0-1023)**
2. **Registered ports (1024-49151)**
3. **Dynamic/private ports (49152-65535)**

### Well-Known Ports

These are commonly used for popular services:

- Port 80: HTTP (web traffic)
- Port 443: HTTPS (secure web traffic)
- Port 22: SSH (secure shell for remote access)
- Port 21: FTP (file transfer protocol)
- Port 25: SMTP (email sending)

---

## Role in Ethical Hacking

Port Scanning is a fundamental technique in ethical hacking used to identify which ports are open on a target system. By discovering open ports, ethical hackers can identify services running on the system and determine if there are any vulnerabilities to exploit.

### Open vs. Closed Ports

- **Open Ports**: Actively accepting connections and can be a gateway for communication. They might be vulnerable if running an outdated or insecure service.
- **ClosedPorts**: Not accepting connections and usually secure from most basic external threats.
- **FilteringPorts**: Firewalls and other security measures can block or filter traffic on certain ports to prevent unauthorized access.

---

## What is Nmap?

**Nmap (Network Mapper)** is an open-source Linux command-line tool used to scan IP addresses and ports in a network and detect installed applications. It allows network admins to find devices on their network, discover open ports and services, and detect vulnerabilities.

### Types of Scans in Nmap

- **SYN Scan**: Also known as "half-open" scanning, this is the most popular form of port scanning. It doesn't complete the TCP handshake, making it less detectable by firewalls.
- **TCP Connect Scan**: Completes the TCP handshake, making it more thorough but more likely to be logged.
- **UDP Scan**: Used to check for open UDP ports.
- **Version Detection**: Determines the software version of services running on open ports.
- **OS Detection**: Identifies the operating system running on a target machine.

---
