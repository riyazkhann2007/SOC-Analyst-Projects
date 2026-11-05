Indicators of Compromise (IOC) Table

Case ID: SOC-PHISH-002
Investigation Type: Malicious URL Threat Intelligence Analysis

1. Identified Indicators

IOC Type| Indicator| Source| Assessment
URL| "hxxps://adcentral[.]com[.]mx/administrator/1new[.]png"| URLhaus, VirusTotal| Malicious
Domain| "adcentral[.]com[.]mx"| URLhaus, VirusTotal| Associated with reported malicious URL
IPv4 Address| "192[.]254[.]185[.]223"| VirusTotal| Observed serving IP
MD5| "96883e2f6d73136f0d181c0ec949a446"| VirusTotal| Favicon hash only
dHash| "645474aa6ac6c948"| VirusTotal| Favicon perceptual hash only

2. Reputation Evidence

- URLhaus listed the URL as an online malware URL.
- VirusTotal reported 15 detections out of 94 security vendors.
- VirusTotal displayed malicious and suspicious classifications.
- The URL returned HTTP status 200 during the recorded analysis.
- VirusTotal associated the URL's crowdsourced context with AgentTesla activity.

3. Important Limitations

- The MD5 and dHash values above belong to the favicon, not the PNG payload.
- No SHA-256 hash of the downloaded PNG payload was obtained.
- The actual payload contents and execution behaviour were not verified.
- The serving IP is an observed infrastructure indicator, not proof that the entire IP address is malicious.
- No endpoint compromise has been confirmed.

4. Recommended SOC Actions

1. Block the URL and assess whether domain-level blocking is appropriate.
2. Search DNS, proxy and endpoint telemetry for matching indicators.
3. Identify whether the URL was accessed or a file was downloaded.
4. Investigate any related process execution or endpoint alerts.
5. Escalate if evidence of compromise is discovered.

5. Investigation Verdict

Verdict: Malicious URL — escalate for further investigation.

Confidence: High confidence in the malicious reputation of the URL based on URLhaus and VirusTotal findings. Payload identity and endpoint impact remain unconfirmed.