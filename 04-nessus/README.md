# Vulnerability Assessment with Nessus

## Objective
Review vulnerability scanner findings and understand how severity labels support remediation prioritisation.

## Evidence
![Nessus vulnerability results](evidence/nessus-results.png)

## Observations
The screenshot shows a scan named `lab vul scan`, one host, and 69 listed vulnerabilities. The visible entries include several Critical and High severity findings. Examples displayed include an Ubuntu Linux issue, a VNC password-related finding, SSL protocol issues, a Samba Badlock finding, an rlogin service detection, and an NFS world-readable share finding.

## Analysis and limitations
These are scanner-reported findings, not independently confirmed vulnerabilities. The screenshot does not show the detailed evidence or remediation for a specific finding, and some rows are truncated. Do not claim that every alert is exploitable without validation.

## Recommendations
Open a finding's detail page, record its exact description and remediation, validate important findings, patch or disable affected services, and rescan after fixes.

## Reference
Tenable Nessus Documentation: https://docs.tenable.com/nessus/

