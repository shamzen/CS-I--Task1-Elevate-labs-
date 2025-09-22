# CS-I--Task1-Elevate-labs
Cyber Security Internship Task 1 - scan Your Local Network for Open Ports

## Tools Used
- **Nmap 7.79** (Port Scanning)
- **Wireshark** (Packet Capture)
- **CMD (Windows)** for IP discovery

---

## Steps

- Identified local IP using:
   ```bash
   ipconfig

- Run a TCP SYN scan on the target:
    ```bash
    nmap -sS <my ip>

- Scan Output:
  ```bash
Starting Nmap 7.97 ( https://nmap.org ) at 2025-09-22 18:49 +0530
Nmap scan report for 172.18.128.1
Host is up (0.000014s latency).
Not shown: 997 closed tcp ports (reset)
PORT    STATE SERVICE
135/tcp open  msrpc
139/tcp open  netbios-ssn
445/tcp open  microsoft-ds

Nmap done: 1 IP address (1 host up) scanned in 0.90 seconds


## Analysis
    ```bash 
   Host: 172.18.128.1
    Open Ports Found:
   135/tcp → Microsoft RPC
    139/tcp → NetBIOS Session Service
    445/tcp → Microsoft SMB


## Risks:
    ```bash 
    SMB ports (139/445)



## Interview Questions

What is an open port?
-An open port is a network port that is active and waiting for incoming connections.

How does Nmap perform a TCP SYN scan?
-Nmap sends a SYN packet, waits for SYN/ACK, then resets without finishing the handshake (stealth scan).

What risks are associated with open ports?
-They can expose services that attackers may exploit if they are weak or outdated.

Explain the difference between TCP and UDP scanning.
-TCP uses a handshake and gives clearer results. UDP has no handshake, so it’s slower and harder to confirm.

How can open ports be secured?
- Close unused ports, update services, use firewalls, and monitor network activity.

What is a firewall's role regarding ports?
-A firewall filters traffic, blocking or allowing connections to protect ports.

What is a port scan and why do attackers perform it?
-A port scan checks for open ports and services. Attackers use it to find weaknesses.

How does Wireshark complement port scanning?
- Wireshark shows the actual packets (SYN, ACK, RST),   helping verify and analyze scans.

### screenshoot

## wireshark 
screenshot: "C:\Users\HP\OneDrive\Desktop\task-1\screenshots\Screenshot 2025-09-22 202341.png"

## Nmap
screenshot: "C:\Users\HP\OneDrive\Desktop\task-1\screenshots\Screenshot 2025-09-22 190203.png"



By:- shivam raj
