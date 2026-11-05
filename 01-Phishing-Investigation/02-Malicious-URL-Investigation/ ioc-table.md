Indicators of Compromise (IOC) Table

Case ID: SOC-PHISH-002

Investigation: Malicious URL Threat Intelligence Analysis

1. URL Indicator

- Type: Malicious URL
- Value: "hxxps://adcentral[.]com[.]mx/administrator/1new[.]png"
- Source: URLhaus and VirusTotal
- Assessment: Reported malicious

2. Domain Indicator

- Type: Domain
- Value: "adcentral[.]com[.]mx"
- Source: URLhaus and VirusTotal
- Assessment: Associated with the reported malicious URL

3. IP Address Indicator

- Type: IPv4 Address
- Value: "192[.]254[.]185[.]223"
- Source: VirusTotal
- Assessment: Observed serving IP during URL analysis

4. Hash Indicators

Favicon MD5:
"96883e2f6d73136f0d181c0ec949a446"

Favicon dHash:
"645474aa6ac6c948"

Important: These hashes identify the favicon, not the suspicious PNG payload. The payload SHA-256 hash was not obtained.

5. Threat Intelligence Findings

- URLhaus listed the URL as an online malware URL.
- VirusTotal reported 15 detections out of 94 security vendors.
- Some vendors classified the URL as malicious, while others marked it suspicious or clean.
- VirusTotal displayed crowdsourced context associating the URL with AgentTesla activity.
- HTTP response status was 200.
- Content type was image/png.

6. Recommended SOC Response

1. Block the URL according to organisational security policy.
2. Search DNS, proxy and endpoint logs for matching indicators.
3. Check whether users accessed the URL.
4. Investigate whether the file was downloaded or executed.
5. Escalate any confirmed endpoint compromise to the incident response team.
6. Preserve the investigation evidence.

7. Final Assessment

Verdict: Malicious URL — escalate for further investigation.

Confidence: High confidence in the malicious reputation of the URL based on URLhaus and VirusTotal evidence.

Limitations: The actual payload was not downloaded or analysed. No endpoint compromise or malware execution has been confirmed.

Investigation Type: Public threat intelligence analysis for educational SOC practice.