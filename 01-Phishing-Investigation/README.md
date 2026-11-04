# Phishing Email Investigation

## Project Objective
To identify and investigate suspicious phishing emails.

## Tools Used
- VirusTotal
- Google Chrome
- GitHub

## Investigation
Test 1: URL Reputation Analysis

URL: https://example.com
Tool: VirusTotal

Result:
- HTTP Status: 200
- Vendor detections: 0
- Domain: example.com

Conclusion:
No security vendors flagged the URL
as malicious in this scan.
## Test 2: URL Threat Detection

URL: https://testsafebrowsing.appspot.com/
Tool: VirusTotal

Findings:
- Webroot: Malicious
- alphaMountain.ai: Suspicious
- Gridinsoft: Suspicious
- Other visible vendors: Clean

Conclusion:
Security vendors flagged this test URL.
It is a controlled security testing site.
Further investigation would be needed before classifying a real-world incident.
## Findings
- Two URLs investigated.
- One URL had zero vendor detections.
- The test URL had malicious and suspicious flags.
- VirusTotal results were documented.

## Conclusion
## Email Authentication Analysis

Sample: Training email
Tool: Gmail Show Original

SPF: PASS
DKIM: PASS
DMARC: PASS

Conclusion:
URL reputation analysis completed.
Two URLs were investigated using VirusTotal.
One URL had zero detections, while the
controlled testing URL triggered suspicious
and malicious vendor flags.
Further investigation is required before
classifying real-world threats.