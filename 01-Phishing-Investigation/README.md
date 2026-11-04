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

Note: This is a controlled security testing URL, not evidence of a real-world malicious website.
## Test 3: Email URL Investigation
### VirusTotal Analysis

- URL: https://learn.microsoft.com/en-gb/training/?wt.mc_id=rmskilling_learn_welcome_email_gdc
- Domain: learn.microsoft.com
- Protocol: HTTPS
- HTTP Status: 200
- Content Type: text/html
- Visible Security Vendor Results: Clean

### Initial Assessment

The URL received clean results from the security vendors visible in the VirusTotal report. The website responded successfully with HTTP status 200.

### Verdict

No suspicious activity was identified in the available VirusTotal results. The URL appears legitimate based on the available evidence, but a clean scan alone cannot guarantee safety.
Conclusion:
Security vendors flagged this test URL.
It is a controlled security testing site.
Further investigation would be needed before classifying a real-world incident 
## Findings
- Two URLs investigated.
- One URL had zero vendor detections.
- The test URL had malicious and suspicious flags.
- VirusTotal results were documented.

## Conclusion
Conclusion:
URL reputation analysis completed.
Two URLs were investigated using VirusTotal.
One URL had zero detections, while the
controlled testing URL triggered suspicious
and malicious vendor flags.
Further investigation is required before classifying real-world threats.
## Email Authentication Analysis

Sample: Training email
Tool: Gmail Show Original

SPF: PASS
DKIM: PASS
DMARC: PASS
## Email Header Investigation

### Sample Details
- Sender: Microsoft Learn
- Domain: notifications.microsoft.com
- Subject: Get started with Microsoft Skilling
- Tool: Gmail Show Original

### Authentication Results
- SPF: PASS
- DKIM: PASS
- DMARC: PASS

### Header Analysis
- Sending IP: 130.248.181.168
- Return-Path: bounce@notifications.microsoft.com
- Email routing: Microsoft infrastructure to Google mail servers.

### Initial Assessment
The email passed SPF, DKIM and DMARC
authentication checks.

The sender domain appears consistent
with Microsoft notification infrastructure.

### Final Verdict
---

## Evidence Screenshots

All investigation screenshots are available below:
1. [Test 1 – Example URL Analysis](evidence/Screenshot_2026-11-04-17-27-38-445_com.miui.gallery-edit.jpg)
2. [Test 2 – Controlled URL Threat Detection](evidence/Screenshot_2026-11-04-17-09-04-352_com.android.chrome.jpg)
3. [Test 3 – Microsoft Learn URL Analysis](evidence/Screenshot_2026-11-04-17-09-04-352_com.android.chrome.jpg)
4. [Email Authentication – SPF, DKIM and DMARC](evidence/)
