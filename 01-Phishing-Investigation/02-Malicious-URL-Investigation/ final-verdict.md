Final SOC Investigation Verdict

Case ID: SOC-PHISH-002

Incident Type: Malicious URL / Threat Intelligence Investigation

Priority: High — Recommended for investigation

Executive Summary

A publicly reported URL hosted on "adcentral.com.mx" was investigated using URLhaus and VirusTotal.

VirusTotal reported 15 detections out of 94 security vendors. URLhaus listed the URL as an online malware URL.

Key Findings

- Malicious URL reputation identified.
- Associated domain and serving IP documented.
- VirusTotal HTTP response and content information recorded.
- Favicon hashes documented separately from payload hashes.
- Evidence screenshots preserved.

Final Verdict

Malicious URL — Escalation recommended.

Confidence is high regarding the URL's malicious reputation.

However, the actual payload identity, endpoint impact and malware execution remain unconfirmed.

Recommended Actions

1. Block the URL according to security policy.
2. Search DNS, proxy and endpoint logs.
3. Identify users or devices that accessed the URL.
4. Investigate downloads and process execution.
5. Escalate confirmed suspicious endpoint activity.
6. Preserve all relevant evidence.

Analyst Conclusion

This investigation demonstrates threat intelligence research, IOC documentation, URL reputation analysis, evidence handling and basic SOC response planning.

Investigation Type: Educational public threat intelligence case study.