# Linux Bootloader Security: GRUB Configuration

## Objective
Understand why physical access to an inadequately protected bootloader can undermine operating-system login controls, and document mitigations for an authorised disposable VM.

## Concepts
GRUB loads the operating system and can expose boot-time recovery options. If an attacker can edit boot parameters and the machine does not enforce suitable bootloader/firmware protections, they may be able to alter the boot path. This is a physical-access and configuration risk, not evidence that every Linux system is vulnerable.

## Safe lab procedure
1. Use a disposable Linux VM that you own and take a snapshot before changing boot settings.
2. Record the Linux distribution/version and the current GRUB configuration state.
3. Review the boot menu and determine whether editing entries is permitted in the current configuration. Do not test this on a shared or production computer.
4. If the lab task requires demonstrating the weakness, follow the instructor-approved recovery demonstration only on the disposable VM. Avoid accessing or copying unrelated personal files.
5. Record what access the configuration permitted and whether the result persisted after a normal reboot.
6. Restore the snapshot or revert all lab changes and verify that the VM boots normally.
7. Document the before/after configuration and the defensive control that prevents the demonstrated path.

## Results and evidence status
No screenshot or result for this exercise was supplied with the portfolio evidence. This entry is a procedure and security analysis, not a claim that root access was obtained.

## Defensive recommendations
Protect firmware settings with a password where appropriate, restrict physical access, configure GRUB authentication for sensitive boot-entry editing, enable Secure Boot where supported, and use full-disk encryption to protect data at rest. These controls address different parts of the threat and should be assessed together.

## Limitations
Bootloader controls vary by distribution and hardware. Full-disk encryption protects stored data but does not replace physical security or boot-chain integrity controls.
