# Basic Network Scanning with Nmap (OASIS INFOBYTE - Task 01)

## Objective

The objective of this task is to perform a basic network scan using Nmap to identify open TCP ports and the services running on the local machine.

## Tool Used

* Nmap 7.99
* Windows Command Prompt

## Command Used

```bash
nmap localhost
```

## Scan Results

```
Starting Nmap 7.99 ( https://nmap.org ) at 2026-06-26 13:52 +0530
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00047s latency).
Other addresses for localhost (not scanned): ::1
Not shown: 997 closed tcp ports (conn-refused)

PORT     STATE SERVICE
135/tcp  open  msrpc
445/tcp  open  microsoft-ds
3306/tcp open  mysql

Nmap done: 1 IP address (1 host up) scanned in 0.31 seconds
```

## Explanation of Open Ports

### Port 135 (MSRPC)

* Service: Microsoft Remote Procedure Call (MSRPC)
* Purpose: Used by Windows for communication between applications and system services.

### Port 445 (Microsoft-DS)

* Service: Microsoft Directory Services (SMB)
* Purpose: Used for Windows file and printer sharing over a network.

### Port 3306 (MySQL)

* Service: MySQL Database Server
* Purpose: Used by the MySQL database to accept client connections.

## Observations

* The localhost machine is active.
* Three TCP ports (135, 445, and 3306) were found to be open.
* Most other TCP ports were closed.
* The scan completed successfully in approximately 0.31 seconds.

## Conclusion

The Nmap scan successfully identified the open ports and their associated services on the local machine. This task demonstrates the use of Nmap as a basic network reconnaissance tool for identifying accessible services and understanding the security posture of a system.

## Author

**Sreedev Sreekumar**

Cybersecurity Internship – Oasis Infobyte

