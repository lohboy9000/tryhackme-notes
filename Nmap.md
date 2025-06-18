# TryHackMe Room: Nmap

## Summary
- Nmap is a network scanning tool used to find open ports and services.
- It helps in the reconnaissance phase of cybersecurity.
- Common scans include stealth SYN (`-sS`), version detection (`-sV`), and aggressive scans (`-A`).
- It reveals what services are running and potential vulnerabilities.

## Cheat Sheet
nmap -sS [IP] # Stealth SYN scan
nmap -sV [IP] # Service version detection
nmap -A [IP] # Aggressive scan (OS detection + scripts)
nmap -p- [IP] # Scan all TCP ports
nmap -Pn [IP] # Skip host discovery

## What I Did
- Scanned target IP with `nmap -sS -p-`.
- Found open ports 22 (SSH) and 80 (HTTP).
- Used `nmap -sV` to get version info.
- Tried aggressive scan with `-A`.
- Need to review UDP scanning next.

## Flashcards
**Q:** What does `nmap -sS` do?  
**A:** Performs a stealth SYN scan to find open ports.

**Q:** When should you use `-Pn`?  
**A:** To skip ping checks when the host does not respond to ICMP.
