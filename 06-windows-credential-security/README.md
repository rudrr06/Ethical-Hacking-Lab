# Windows Credential Storage Security: SAM and Hashdump Concepts

## Objective
Understand where Windows local account credential material is protected and why credential-dumping output must be handled as highly sensitive data.

## Concepts
The Security Account Manager (SAM) database stores local account password hashes, not plaintext passwords. Access to the SAM and related system secrets is restricted by Windows and may be affected by privilege level, system state, and security controls. A hash is still sensitive and must not be published.

## Safe procedure for an authorised lab
1. Use a disposable Windows VM with dummy local accounts and take a snapshot.
2. Record the Windows edition/version and whether the account under test is local or domain-managed.
3. Review the security controls relevant to credential access, including administrator privileges, endpoint protection, and credential-protection features.
4. If the class exercise includes a credential-access demonstration, perform only the instructor-approved method against the disposable VM and dummy accounts.
5. Do not copy SAM/SYSTEM files, export hashes into the portfolio, or attempt to crack real users' credentials.
6. Record only non-sensitive observations: whether access was blocked or allowed, which defensive control was relevant, and the system state.
7. Revert the VM snapshot and remove any lab artefacts after the exercise.

## Results and evidence status
No screenshot or specific result was supplied. This report does not claim that hashes were extracted or cracked.

## Defensive recommendations
Use least privilege, strong unique passwords, endpoint detection and response, timely security updates, and available Windows credential protections. Monitor suspicious access to credential stores and investigate unexpected administrative activity.

## Limitations
Credential protections differ across Windows versions and configurations. A single lab result should not be generalised to every Windows installation.
