# Payload Formats and Callback Concepts

## Objective
Document a lab exercise demonstrating generation of a Linux ELF-format payload and discuss the security implications of executable payloads.

## Evidence
![Payload generation output](evidence/payload-generation.png)

## Observation
The terminal output shows `msfvenom` reporting a Linux x86 Meterpreter reverse-TCP payload and a generated ELF file named `vir.elf`. The output reports a payload size of 123 bytes and a final ELF file size of 207 bytes.

## Analysis and limitations
This screenshot demonstrates file generation output only. It does not, by itself, establish that the payload executed successfully or that a remote session was established. The payload file itself should not be published.

## Defensive considerations
Keep endpoint protection enabled, isolate lab virtual machines, restrict untrusted executable files, and monitor unexpected outbound connections.

## Reference
Metasploit Documentation: https://docs.metasploit.com/

