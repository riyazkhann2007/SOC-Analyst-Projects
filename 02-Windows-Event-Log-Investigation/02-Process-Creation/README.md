Windows Process Creation Investigation

1. Objective

Investigate Windows process creation events to identify potentially suspicious process activity.

2. Event ID Analysed

Event ID| Description
4688| A new process has been created

3. Fields to Examine

- Process name
- Process ID
- Creator process ID
- Parent process name
- Command-line arguments
- Event timestamp

4. Investigation Approach

- Identify newly created processes.
- Examine parent and child process relationships.
- Review unusual process names.
- Analyse suspicious command-line arguments.
- Correlate process activity with login events.

5. Investigation Status

Pending — Sample event analysis.

6. Data Source

Educational sample and simulated Windows Security Event Logs.

7. Disclaimer

This investigation uses simulated data for educational purposes and does not represent activity collected from a real production system.