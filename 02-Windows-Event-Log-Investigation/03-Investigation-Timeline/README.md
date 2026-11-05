Windows Security Investigation Timeline

1. Objective

Create a chronological timeline of Windows Security Events to understand the sequence of suspicious activities.

2. Events to Correlate

- Event ID 4625 — Failed logon
- Event ID 4624 — Successful logon
- Event ID 4688 — Process creation
- Event ID 4672 — Special privileges assigned

3. Timeline Fields

- Date and timestamp
- Event ID
- Account name
- Source IP address
- Process name
- Activity description

4. Investigation Method

- Arrange events by timestamp.
- Identify repeated authentication failures.
- Check for successful logons following failures.
- Correlate login activity with process creation.
- Document suspicious sequences.

5. Investigation Status

Pending — Sample timeline creation.

6. Data Source

Educational sample and simulated Windows Security Event Logs.

7. Disclaimer

The timeline will be based on simulated data and is intended for educational SOC investigation practice.