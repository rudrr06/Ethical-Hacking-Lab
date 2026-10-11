# SQL Injection: Demonstration and Prevention

## Objective
Understand how unsafe construction of SQL statements can allow user input to alter query logic, and explain how parameterised queries prevent this class of injection.

## Concepts
SQL injection can occur when untrusted input is concatenated directly into a SQL statement. A secure application separates query structure from input values by using parameterised queries/prepared statements. Input validation is useful but is not a substitute for parameterisation.

## Safe lab procedure
1. Start a deliberately vulnerable training application in a local, isolated VM or container, using dummy data only.
2. Confirm the target URL and database are part of the lab and contain no real user records.
3. Submit a normal, benign value and record the baseline response.
4. Follow the training application's approved SQL-injection exercise using non-destructive test inputs supplied by the lab. Do not test real websites or attempt data extraction from systems outside the scope.
5. Compare the response with the baseline and capture only the minimum evidence needed to explain whether input appears to alter query behaviour.
6. Inspect the application's query-handling code if available and identify whether it concatenates input or uses parameters.
7. Replace unsafe string construction with a parameterised query in the lab code, if the exercise includes remediation.
8. Repeat the same benign test to confirm normal behaviour and record the change.
9. Reset the training database and redact any personal or secret data before saving evidence.

## Results and evidence status
No screenshot or specific test result was supplied for this portfolio entry. This report explains the procedure and defensive concept; it does not claim that SQL injection was successfully demonstrated on a particular application.

## Defensive recommendations
Use prepared statements/parameterised queries, least-privilege database accounts, safe error handling, and regression tests. Do not rely on filtering a few suspicious characters as the primary defence.

## References
[OWASP SQL Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)
