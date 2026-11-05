Malicious URL Investigation Report

1. Case Information

- Case ID: SOC-PHISH-002
- Investigation Type: Malicious URL Analysis
- Priority: High
- Status: Escalated for further investigation
- Analyst: Junior SOC Analyst
- Data Source: URLhaus and VirusTotal

2. Investigation Objective

Investigate a publicly reported suspicious URL using threat intelligence sources, identify associated indicators, assess its reputation, and recommend appropriate SOC response actions.

3. Initial Indicator

URL:

"hxxps://adcentral[.]com[.]mx/administrator/1new[.]png"

4. Investigation Findings

URLhaus

- The URL was listed in the URLhaus malware URL database.
- The listing displayed an Online status.
- Malware-related tags were visible in the database listing.

VirusTotal

- Detection ratio: 15/94.
- Some security vendors classified the URL as malicious or suspicious.
- HTTP response: 200.
- Content type: image/png.
- Observed serving IP: "192[.]254[.]185[.]223".
- Crowdsourced context displayed an association with AgentTesla activity.

5. Indicators Identified

- URL: "hxxps://adcentral[.]com[.]mx/administrator/1new[.]png"
- Domain: "adcentral[.]com[.]mx"
- IP address: "192[.]254[.]185[.]223"
- Favicon MD5: "96883e2f6d73136f0d181c0ec949a446"
- Favicon dHash: "645474aa6ac6c948"

The hash values identify the favicon, not the suspicious PNG payload.

6. Security Assessment

The URL has a malicious reputation supported by its URLhaus listing and VirusTotal detections.

The AgentTesla association is contextual threat-intelligence information and does not independently confirm the payload identity.

No endpoint logs were available to establish whether a user accessed the URL or whether malware executed.

7. Recommended Response Actions

1. Block the URL according to organisational policy.
2. Search DNS, proxy and endpoint logs for matching indicators.
3. Identify affected users or endpoints, if any.
4. Check for downloaded files and suspicious process execution.
5. Escalate confirmed suspicious endpoint activity to the incident response team.
6. Preserve evidence for further analysis.

8. Final Verdict

Malicious URL — Escalate for further investigation.

Confidence: High confidence in the malicious reputation of the URL.

Impact: Unknown. No endpoint compromise has been confirmed.

9. Lessons Learned

- Correlate multiple threat-intelligence sources instead of relying on one detection score.
- A successful HTTP response does not mean a URL is safe.
- Always distinguish file hashes from favicon hashes.
- Threat-intelligence reputation alone cannot prove endpoint compromise.
- SIEM monitoring can help identify access to known malicious indicators.

10. Investigation Limitations

This was an educational public threat-intelligence investigation. No suspicious URL was directly opened, no payload was downloaded, and no production endpoint was accessed.