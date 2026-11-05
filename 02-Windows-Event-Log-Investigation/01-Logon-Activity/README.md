Windows Logon Activity Investigation

1. Objective

Analyse Windows authentication events to identify failed logins, successful logins, and potentially suspicious login patterns.

2. Event IDs Analysed

Event ID| Description
4624| Successful logon
4625| Failed logon

3. Log Fields to Examine

- Timestamp
- Account name
- Source IP address
- Logon type
- Failure reason
- Workstation name

4. Investigation Approach

- Review failed login events.
- Identify repeated authentication failures.
- Check whether a successful login follows failed attempts.
- Compare usernames, timestamps and source IP addresses.
- Determine whether activity requires further investigation.

5. Investigation Status

Pending — Sample event analysis.

6. Data Source

Educational sample and simulated Windows Security Event Logs.

7. Disclaimer

This investigation is for educational purposes. The sample events do not represent activity collected from a real production system.