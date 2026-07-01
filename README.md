# email-analysis-task2

## Overview

This task analyzes a historical email communication and evaluates its security posture using modern email authentication standards. The objective is to identify potential phishing indicators, spoofing attempts, and authentication issues by examining email headers and security controls such as SPF, DKIM, and DMARC.

---

## Objective

- Analyze email header information.
- Evaluate SPF, DKIM, and DMARC authentication mechanisms.
- Identify signs of phishing, spoofing, or malicious activity.
- Document findings in a professional forensic report.

---

## Email Details

| Field | Value |
|---------|---------|
| Sender | john.monaco@citi.com |
| Recipient | robert.badeer@enron.com |
| Subject | RE: RE: Whats up!!!!! |
| Date | Fri, 8 Mar 2002 12:53:01 -0800 (PST) |

---

## Tools Used

- MXToolbox Header Analyzer
- Email Header Analysis Techniques
- Web Browser

---

## Authentication Results

### DMARC

**Status:** Failed

Policy Detected:

```text
v=DMARC1; p=reject
```

The analyzed message was not DMARC compliant according to modern validation checks.

### SPF

**Status:** Failed

SPF record was identified, but authentication validation failed.

### DKIM

**Status:** Failed

No DKIM signature was found in the analyzed message.

---

## Security Analysis

### Sender Verification

- Sender domain: citi.com
- Recipient domain: enron.com
- No evidence of domain impersonation was observed.

### URL Analysis

- No suspicious or obfuscated URLs were identified.
- No malicious redirection attempts were detected.

### Social Engineering Indicators

The message was reviewed for:

- Urgent requests
- Threats
- Financial scams
- Credential harvesting attempts

**Result:** No phishing indicators found.

### Content Review

The email appears to be a normal business conversation involving:

- Corporate transition information
- Employee communication
- Trading-related discussion

---

## Important Note

This email originates from **March 2002**.

Modern email authentication technologies such as SPF, DKIM, and DMARC were not widely deployed at that time. Therefore, authentication failures reported by modern analysis tools should not automatically be interpreted as evidence of phishing or spoofing.

---

## Findings

| Check | Result |
|---------|---------|
| SPF Authentication | Failed |
| DKIM Authentication | Failed |
| DMARC Compliance | Failed |
| Malicious Links | Not Detected |
| Credential Theft Indicators | Not Detected |
| Domain Spoofing Evidence | Not Detected |

---

## Conclusion

The analyzed email appears to be a legitimate historical business communication. Although SPF, DKIM, and DMARC checks fail when evaluated using modern security standards, these failures are expected due to the age of the email. No significant indicators of phishing, malware distribution, or email spoofing were identified.

**Final Verdict:** Legitimate historical email with no evidence of active phishing or malicious intent.

---

## Author

Ashraf Hussain
