# Cybersecurity Labs

Beginner-level cybersecurity portfolio documenting lab exercises in reconnaissance, network scanning, vulnerability assessment, Linux/Windows security, post-exploitation concepts, traffic analysis, and web application testing.

> **Scope and evidence standard:** Each entry separates what the supplied evidence shows from general procedure and defensive analysis. A missing screenshot/result is explicitly labelled; it is not represented as a completed finding. All testing must be performed only on owned systems or targets with explicit authorisation.

## Projects with supplied screenshot evidence
- [Google Dorking for Public Document Discovery](01-google-dorking/README.md)
- [Network Scanning with Nmap](03-nmap/README.md)
- [Vulnerability Assessment with Nessus](04-nessus/README.md)
- [Linux Bootloader Security: GRUB](05-grub/README.md) — procedure guide; no evidence supplied
- [Windows Credential Storage Security](06-windows-credential-security/README.md) — procedure guide; no evidence supplied
- [Post-Exploitation Concepts with Meterpreter](07-meterpreter/README.md)
- [Payload Formats and Reverse-Connection Concepts](08-payload-formats/README.md)
- [Remote Administration with Radmin](09-radmin/README.md) — procedure guide; no evidence supplied
- [Phishing Simulation and Credential-Safety Awareness](10-phishing-awareness/README.md) — redacted evidence
- [Network Traffic Analysis with Wireshark](11-wireshark/README.md) — redacted evidence
- [Web Application Scanning with OWASP ZAP](12-owasp-zap/README.md)
- [SQL Injection: Demonstration and Prevention](13-sql-injection/README.md) — procedure guide; no evidence supplied
- [Open-Source Intelligence (OSINT) Investigation](02-osint/README.md) — procedure guide; no evidence supplied

## Tools represented
Nmap, Tenable Nessus, Metasploit/Meterpreter, Wireshark, OWASP ZAP, Google Search operators, and OSINT Framework. Tools are listed only in the context supported by the included report/evidence.

## How to read these reports
Each project includes an objective, relevant concepts, scope, numbered procedure, observations/evidence status, interpretation, limitations, and defensive recommendations. Steps that describe a repeatable method are not a claim that every step was performed in the original session. Where no result evidence was supplied, the report says so explicitly.

## Public-release hygiene
- The SocialPhish and Wireshark screenshots have been redacted to obscure credential-like values and network identifiers.
- Do not add payload binaries, credentials, hashes, private captures, or unredacted originals.
- Keep any further screenshots limited to dummy data and approved lab systems.
- Before publishing, confirm that the target and all captured traffic were authorised for the exercise.

## Disclaimer
These materials are for education and authorised security testing only. Never test systems without explicit permission.
