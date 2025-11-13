# Analysis of Nmap Scan Results

## 1. Network Range Scanned
(Note: The network range used is an example)
I scanned the network: 192.168.0.0/24 

## 2. Live Hosts Detected
(Note: The used ip address is an example)
Nmap was able to identify active devices on my network such as:
- 192.168.0.1 → Router
- 192.168.0.16 → My Linux Mint laptop

## 3. Open Ports and Services
Nmap scanned the top 1000 TCP ports on my laptop and reported:

- **All 1000 scanned ports on kishor-HP-246-Notebook-PC (192.168.0.16) are in ignored states.**
- **Not shown: 1000 closed tcp ports (reset)**

This indicates:
- My laptop is not running any network services like SSH, HTTP, FTP, etc.
- The firewall or NAT is blocking unsolicited traffic.
- The system is following a secure default configuration.

## 4. Potential Security Risks
Since no ports are open:
- There is **no direct remote-access risk**
- Attack surface is **minimal**
- Firewall rules appear to be functioning correctly
- This is a secure setup for everyday usage

Any risks would depend on the router or other devices, not my laptop.

## 5. Conclusion
The scan shows that my laptop has no exposed TCP services. This is normal for Linux Mint and indicates strong security by default. The task helped me understand host discovery, scanning, and analyzing open ports even if none were present.

