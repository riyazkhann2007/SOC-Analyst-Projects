SIEM Detection – Malicious URL Access

Objective

Create a sample Splunk detection query to identify endpoints accessing known malicious URLs.

Detection Scenario

An endpoint accesses a URL listed in a threat-intelligence feed.

Splunk SPL Query

index=proxy_logs
| search url="*adcentral.com.mx*"
| stats count values(url) AS requested_urls values(src_ip) AS source_ips values(user) AS users by dest
| where count >= 1

Detection Logic

- Search proxy logs for requests containing the investigated domain.
- Identify the destination, source IP and associated user.
- Generate an alert for analyst review when a matching request is found.

Suggested Alert Details

- Alert name: Known Malicious URL Access
- Suggested severity: High
- Data source: Web proxy logs
- Recommended action: Investigate the source endpoint and user activity.

Investigation Steps

1. Identify the endpoint and user.
2. Confirm the URL against current threat intelligence.
3. Check whether a file was downloaded.
4. Review endpoint alerts and process activity.
5. Escalate if evidence of compromise is identified.

Testing Status

This is an example Splunk SPL query for educational purposes. It has not been executed against a live Splunk environment. The index and field names must be adapted to the organisation's actual data.

Expected SOC Outcome

The query should identify matching proxy events and provide context for further investigation.
