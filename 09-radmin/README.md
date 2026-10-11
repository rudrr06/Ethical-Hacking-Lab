# Remote Administration with Radmin

## Objective
Understand how remote-administration software enables legitimate support and why installation, authentication, and network exposure must be controlled.

## Concepts
Remote administration tools can provide interactive access to another computer. The security risk depends on whether the tool is installed with the owner's consent, correctly authenticated, patched, logged, and restricted to trusted networks.

## Safe lab procedure
1. Use two lab machines that you own or are authorised to administer; do not install a remote-control service on another person's device.
2. On the designated host, record whether the Radmin Server component is installed and which service/port is configured, without recording passwords or licence keys.
3. Review the server's access-control settings and permit only a designated test account.
4. From the authorised client, attempt the approved connection and record whether access is granted or denied. Use dummy lab credentials only.
5. Confirm that the session provides only the expected level of access and that the connection is logged where logging is available.
6. Disconnect the client and disable or uninstall the service if it is not required for the lab.
7. Verify that the host no longer accepts remote connections on the service's port, using the operating system's service/firewall view.

## Results and evidence status
No screenshot or concrete result was provided for this portfolio entry. It does not claim that a Radmin connection was successfully made.

## Defensive recommendations
Use strong unique credentials, restrict source IPs with firewall rules or VPN access, keep the software updated, monitor connection logs, and remove remote administration software that is not needed.

## Limitations
This is a procedure guide. Add a dated screenshot or a short factual result only after the exercise has actually been completed and verified.
