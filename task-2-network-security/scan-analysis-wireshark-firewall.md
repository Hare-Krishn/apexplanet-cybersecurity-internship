# Wireshark Packet Analysis

## Traffic Captured
- HTTP traffic
- DNS queries
- FTP communication
- ICMP packets

## Observations
- DNS queries show domain resolution process
- HTTP traffic visible in plaintext
- FTP credentials transmitted without encryption
- ICMP packets observed during ping scans

## SYN Flood Analysis
- SYN packets analyzed during simulated attack
- Demonstrated excessive connection requests

## Conclusion
Packet analysis highlights risks of unencrypted protocols
and importance of traffic monitoring.


# Firewall Basics – Task 2

## Objective
Demonstrate basic firewall rules and block a port scan.

## Firewall Rule Used
```bash
iptables -A INPUT -p tcp --dport 22 -j DROP
```

## Verification
```bash
iptables -L -n
```
## Result
- SSH port (22) was blocked  
- Nmap scan showed the port as **filtered**

## Conclusion
`iptables` successfully blocked unauthorized access to the service.
