## What is Scanning

Scanning is a set of procedures for: 
- identifying live hosts, ports, and services
- discovering the OS of the target system
- identifying vulnerabilities and threats in the network

## Scanning Types

Scanning is classified as **active** or **passive**
- **Passive Scanning**: Scanning a network without directly interacting with the target device. Usually carried out through packet capture and analysis tools like Wireshark. 
- **Active Scanning**: Scanning individual endpoints in an IT network to retrieve more detailed information. Involves sending packets or queries dfirectly to assets rather than passively collecting data in transit.

## Scanning Techniques

### Network Scanning
A network is usually a collecton of interconnected hosts/computers that share information and resources.

Network scanning helps to discover and map a complete network, including:
- live computers or hosts
- open ports
- IP addresses
- services running on any live host and OS

### Port Scanning
Port scanning examines open ports in a network capable of receiving and sending data.

Port numbers varies between **0 to 65,536**. Scanning results fall into the following categories:
- **Closed Ports**: host is not listening on the port
- **Open Ports**: host is actively accepting connection
- **Filtered Ports**: the port is open however the host is not accepting connections or is accepting based on criteria (e.g., source IP address)

### Vulnerability Scanning
Vulnerability scanning proactively identifies the network's vulnerabilities to determing if the system may be threatened or exploited.

Pentesteres widely use tools like [Nessus](https://www.tenable.com/products/nessus) and [Acunetix](https://www.acunetix.com/) to identify loopholes in a system.

## Scanning Tools

### Network Mapper (Nmap)
Nmap is a popular tool used to carry out port scanning, discover network protocols, identify running services, and detect operating systems on live hosts. 

Some important Nmap options:
- **TCP SYN Scan**: get the list of live hosts and associated ports on the hosts without completing the TCP three-way handshake, making scan a little stealthier.
	- Usage: **`nmap -sS MACHINE_IP`**
- **Ping Scan**: Allows scanning live hosts in network without going deeper and checking for ports
	- Usage: **`nmap -sn MACHINE_IP
- **Operating System Scan**: Allows scanning of the type of OS running on a live host. 
	- Usage: **`nmap -O MACHINE_IP`.**
-   **Detecting Services**: Get a list of running services on a live host.
	- Usage: **`nmap -sV MACHINE_IP`**

### Nikto
Nikto allows scanning websites for vulnerabilities. It enables looking for subdomains, outdated servers, debug messages, etc on a website.

**`nikto -host 10.10.60.101`**


## Further TryHackMe Resources

- Namp module: https://tryhackme.com/module/nmap
	- [Nmap](https://tryhackme.com/room/furthernmap), 
	- [Nmap live host discovery](https://tryhackme.com/room/nmap01)
	- [Nmap basic port scan](https://tryhackme.com/room/nmap02) 
	- [Nmap advanced port scan](https://tryhackme.com/room/nmap03)
