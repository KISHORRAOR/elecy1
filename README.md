# Task 1 – Network Port Scanning

## Objective
Scan local network for open ports and services to understand network exposure.

## Tools Used
- Nmap
- Wireshark (optional)

## Commands Run
- Discover live hosts (ping sweep):
  `sudo nmap -sn NETWORK_RANGE -oG hosts_up.gnmap`
- SYN scan (conservative):
  `sudo nmap -sS -T3 --max-retries 2 NETWORK_RANGE -oA scan_results`
- (Optional) Service/version scan for a host:
  `sudo nmap -sS -sV -p 1-1000 -T3 <host-ip> -oN host_services.txt`

## Files included
- `scan_results.nmap`, `scan_results.xml`, `scan_results.gnmap`
- `analysis.md`
- `screenshots/` (terminal output images)

## Notes
All scans were performed only on devices I own.
