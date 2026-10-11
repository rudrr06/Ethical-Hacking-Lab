# Network Scanning with Nmap

## Objective
Identify open TCP ports and reported service/version information on an authorised lab host.

## Method
The screenshot shows an Nmap service/version scan against a lab host at `192.168.56.101`.

## Evidence
![Nmap scan output](evidence/nmap-scan.png)

## Observations
The output reports the host as up and lists multiple open TCP services, including FTP, SSH, Telnet, SMTP, DNS, HTTP, SMB, database services, and others. The scan reports 977 closed TCP ports in the default scanned range.

## Analysis and limitations
Service/version detection is indicative, not definitive proof of a vulnerability. The displayed target appears to be a lab machine; keep testing restricted to systems you own or are authorised to assess. The screenshot includes an internal lab IP and a MAC address; consider redacting them before public release.

## Recommendations
Disable unnecessary services, restrict management interfaces, patch exposed services, and validate findings with the system owner.

## Reference
Nmap Reference Guide: https://nmap.org/book/man.html

