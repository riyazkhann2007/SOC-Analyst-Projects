SOC Detection Ideas – Malicious URL Investigation

Case ID

SOC-PHISH-002

Objective

Define practical detection ideas that could help a SOC team identify access to known malicious URLs and related suspicious activity.

1. Known Malicious URL Access

Detection logic:

- Monitor proxy, DNS and web gateway logs.
- Compare requested URLs and domains against approved threat-intelligence feeds.
- Generate an alert when an endpoint accesses a known malicious indicator.

Suggested severity: High

2. Suspicious File Download

Detection logic:

- Monitor downloads from known malicious domains.
- Investigate unexpected executable, script or archive downloads.
- Correlate download activity with endpoint security alerts.

Suggested severity: High

3. Suspicious Process Execution

Detection logic:

- Review process creation events, including Windows Event ID 4688.
- Investigate unexpected PowerShell or command prompt execution after suspicious web activity.
- Correlate process execution with the affected user and endpoint.

Suggested severity: Medium to High

4. Multiple Security Signals

Increase investigation priority when multiple indicators occur together:

- Access to a known malicious URL.
- Suspicious file download.
- Endpoint malware detection.
- Unexpected process execution.

5. False Positive Considerations

- Threat-intelligence feeds may contain outdated indicators.
- Shared hosting IP addresses may serve legitimate websites.
- A URL reputation match does not prove malware execution.
- Validate the indicator and investigate endpoint context before escalating.

6. Analyst Recommendation

Use threat-intelligence enrichment, web proxy monitoring, DNS monitoring and endpoint detection alerts to improve malicious URL detection.

Implementation status: Detection concepts documented for educational purposes. No production SIEM rule has been deployed or tested.