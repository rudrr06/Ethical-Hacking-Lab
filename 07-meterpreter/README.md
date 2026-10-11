# Post-Exploitation Concepts with Meterpreter

## Objective
Document the basic directory-enumeration activity visible in an authorised Metasploitable lab session and explain why post-exploitation access must be tightly scoped.

## Concepts
Meterpreter is a Metasploit payload/session interface used in authorised penetration tests. Post-exploitation enumeration can reveal the account context and accessible files. The available commands and access depend on the session type and permissions.

## Lab environment and scope
The screenshot shows a Meterpreter prompt and a directory listing for `/home/msfadmin`. This is consistent with a lab target such as Metasploitable. The screenshot does not show enough context to establish every step used to obtain the session.

## Procedure: session verification and basic enumeration
1. Start only the isolated, intentionally vulnerable lab VM and the authorised testing VM; verify they are on the intended host-only or isolated network.
2. Establish a session using the lab's instructor-approved exploitation method. Do not deploy a payload to a third-party or production system.
3. Confirm that the session prompt is active and identify the session type using the framework's session information.
4. Record the current user/context and basic system details using the session's built-in information commands.
5. List the contents of the approved lab user's home directory. Do not open or copy unrelated personal data.
6. Record filenames and permissions only when they help explain the lab objective; avoid including secrets in screenshots.
7. Exit the session when the required enumeration is complete and shut down or revert the lab VM.
8. Record the access obtained, the minimum evidence supporting it, and the defensive lesson. Do not claim persistence, privilege escalation, or data exfiltration unless those actions were separately authorised and evidenced.

## Observed result
The supplied screenshot shows a Meterpreter prompt and a directory listing for `/home/msfadmin`, including filenames and permission information. It supports the claim that a session was available and basic directory enumeration was performed. It does not prove persistence, elevated privileges, or broader network access.

## Evidence
![Meterpreter session and directory listing](evidence/meterpreter-enumeration.png)

## Defensive analysis
Unexpected remote sessions can indicate successful exploitation. Apply least privilege, segment vulnerable systems, patch exposed services, monitor unusual process/network activity, and investigate unauthorised remote access.

## Reference
[Metasploit Documentation](https://docs.metasploit.com/)
