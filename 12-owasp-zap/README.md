# Web Application Scanning with OWASP ZAP

## Objective
Review alerts reported by a web application scanner and understand their limits.

## Evidence
![Web scanner alerts](evidence/owasp-zap-alerts.png)

## Observations
The screenshot displays 11 alerts, including missing security headers, cookie configuration concerns, possible information disclosure, and session-management-related alerts. The scan interface shows `http://testfire.net` as the target.

## Analysis and limitations
These are scanner-reported alerts and require review. The screenshot does not show the detail page for an individual alert, so its evidence, confidence, and remediation cannot be fully assessed here. Ensure the target was explicitly authorised for the testing performed.

## Recommendations
Open an alert detail, record its risk and confidence, validate it in scope, and document a specific remediation. Do not claim the scan confirms exploitability based on the summary alone.

## Reference
OWASP ZAP Documentation: https://www.zaproxy.org/docs/

