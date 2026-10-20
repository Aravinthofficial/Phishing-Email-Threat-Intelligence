# Phishing-Email-Threat-Intelligence

## Project Overview
This project investigates a suspicious email using email header analysis, IOC extraction, and threat intelligence tools.

## Objectives
- Analyze sender, subject, and email headers.
- Extract URL, domain, IP address, and SHA-256 hash.
- Investigate suspicious indicators using security tools.
- Map relevant behavior to MITRE ATT&CK.
- Prepare a phishing incident report.

## Tools Used
- VirusTotal
- URLScan
- AbuseIPDB
- WHOIS / DNS (MXToolbox)
- MITRE ATT&CK
- Email Header Analysis

## Investigation Workflow
1. Collect and preserve the sample email.
2. Analyze email headers and authentication results.
3. Extract Indicators of Compromise (IOCs).
4. Check IP, domain, and URL reputation.
5. Review DNS and domain registration information.
6. Map relevant phishing techniques.
7. Prepare the incident report.

## Key Findings
- Sender: `banco.bradesco@atendimento.com.br`
- Sending IP: `137.184.34.4`
- SPF: `temperror`
- DKIM: `none`
- DMARC: `temperror`
- Suspicious domain: `blog1seguimentmydomaine2bra[.]me`
- Attachment: None identified

## Final Verdict
**Suspicious — Likely Phishing**

The email uses an urgent rewards-expiry message and a destination domain that does not obviously match the displayed brand. Email authentication results also require further investigation.

This is a preliminary assessment, not confirmation that the infrastructure is currently malicious.

## Screenshots
Screenshots of email headers, VirusTotal, AbuseIPDB, URLScan, DNS lookups, and MITRE ATT&CK are included in the `screenshots/` folder.

## Incident Report
See `reports/incident-report.pdf` for detailed findings, evidence, limitations, and recommended response actions.

## Disclaimer
This project uses a public historical email sample for educational purposes. URLs are defanged for safety. No recipient compromise is claimed.

