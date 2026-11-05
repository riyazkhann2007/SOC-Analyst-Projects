Windows Security Event Dataset Description

Dataset Overview

This dataset contains simulated Windows Security Event records created for educational SOC investigation practice.

Dataset File

"windows_security_events.csv"

Event IDs Included

Event ID| Description
4624| Successful logon
4625| Failed logon
4672| Special privileges assigned
4688| Process creation

Dataset Fields

- Timestamp
- Event ID
- Username
- Source IP
- Logon Type
- Process Name
- Parent Process
- Description

Investigation Scenario

The dataset simulates repeated failed login attempts against an admin account, followed by a successful login, privilege assignment and process creation activity.

Important Notes

- All records are simulated.
- The IP address "203.0.113.50" is reserved for documentation examples.
- The dataset is not extracted from a real Windows machine.
- The records are designed for learning event correlation and SOC investigation.

Purpose

To practise Windows event analysis, authentication monitoring, process investigation and security reporting.