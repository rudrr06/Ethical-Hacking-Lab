# Phishing Simulation and Credential-Safety Awareness

## Objective
Examine the visible workflow of a phishing-simulation tool and demonstrate why credential collection must be limited to a controlled, consent-based awareness exercise.

## Scope and safety
This portfolio describes a local lab demonstration only. Use dummy values and systems you control. Do not send phishing links to real users, impersonate a service without permission, or collect real passwords. The evidence image has been redacted before public release; the original should remain private.

## Procedure: safe awareness simulation
1. Confirm written authorisation, scope, and the test audience before starting any simulation.
2. Use a local-only or purpose-built training environment, with network access restricted to the lab.
3. Select a simulation template only for the approved training objective; do not publish or distribute a live credential-harvesting URL.
4. Use a clearly identified test account and dummy password, never a real account.
5. If the exercise records a submission, verify only that the dummy event was registered. Do not store or display the submitted password.
6. Stop the simulation, remove stored test records, and confirm that no public listener or tunnel remains active.
7. Capture redacted evidence that demonstrates the training workflow without showing credentials, URLs that could still be reached, or personal information.
8. Report the defensive lesson: recognise suspicious domains, avoid entering credentials from unexpected links, and report suspected phishing through the approved channel.

## Observed result
The screenshot shows the SocialPhish terminal interface, a local URL, client activity, and output indicating that test input was saved. It originally displayed password-like data and a saved-record path; those regions are obscured in this portfolio copy. The screenshot is not evidence of a real-world campaign or successful compromise.

## Evidence
![Redacted local phishing-simulation output](evidence/socialphish-lab.png)

## Analysis and recommendations
Credential-harvesting tools can expose secrets if misused or misconfigured. Use approved awareness platforms, dummy data, phishing-resistant MFA where possible, secure deletion of simulation records, and clear reporting procedures.

## Reference
[CISA: Recognize and Report Phishing](https://www.cisa.gov/secure-our-world/recognize-and-report-phishing)
