# SOC L1 Alert Triage – True Positive Investigation

## Overview

This write-up documents a Security Operations Centre (SOC) Level 1
alert triage investigation completed in the TryHackMe SIEM environment.

The objective was to investigate a suspicious security alert, review
the available evidence, identify relevant Indicators of Compromise
(IoCs), use external threat intelligence to validate the findings,
and determine the appropriate alert verdict.

**Final Verdict:** True Positive

---

## Investigation Summary

**Environment:** TryHackMe

**Platform:** TryHackMe SIEM

**Investigation Type:** SOC L1 Alert Triage

**Analyst:** Olawale Otasanya

**Alert Classification:** True Positive

**Investigation Status:** Completed

**Final Action:** Alert Closed

---

## 1. Alert Overview

I began the investigation by reviewing the alert within the TryHackMe
SIEM.

I examined the available alert information, including the alert
severity, description and associated details, to understand why the
activity had been detected and determine what information required
further investigation.

### Alert Overview

<img width="1917" height="822" alt="Screenshot 2026-07-28 093813" src="https://github.com/user-attachments/assets/f3e55078-b5a4-4ced-b16b-fb72ab05817c" />


The alert contained information that could be used to investigate the
activity further, including details relating to the suspicious file
and associated activity.

---

## 2. Investigation

I opened the alert and reviewed the available investigation details.

During the investigation, I identified a file hash associated with the
suspicious activity. The hash was treated as an Indicator of Compromise
(IoC) and was used for further analysis.

The investigation focused on:

- Alert details and severity
- Suspicious file information
- File hash
- Associated activity
- Available network or event information
- Evidence that could support or contradict the alert

### Investigation Details

<img width="1917" height="542" alt="Screenshot 2026-07-28 093954" src="https://github.com/user-attachments/assets/3b6d1397-491c-4f1d-9be1-d1cafa83f883" />


The identified file hash provided an opportunity to perform additional
threat intelligence analysis and validate whether the file had
previously been identified as malicious.

---

## 3. Indicator of Compromise – File Hash

A file hash associated with the suspicious activity was identified
during the SIEM investigation.

Rather than relying solely on the original SIEM alert, I used the hash
as an IoC to perform an external threat intelligence lookup.

This provided an additional source of evidence to help determine
whether the alert represented genuine malicious activity.

---

## 4. Threat Intelligence Analysis

I submitted the identified file hash to VirusTotal to determine whether
the file had previously been detected by security vendors.

The VirusTotal analysis returned:

**49 / 70 security vendors flagged the file as malicious.**

The sample was also associated with the **LummaStealer** malware family,
with detections including Trojan and spyware classifications.

### VirusTotal Analysis

<img width="1917" height="867" alt="Screenshot 2026-07-28 094127" src="https://github.com/user-attachments/assets/a94fcff6-1079-4f57-b8dd-38b252279b27" />


The results provided strong supporting evidence that the identified
file was malicious.

The VirusTotal results were considered alongside the original SIEM
alert rather than being treated as the only source of evidence.

---

## 5. Analysis

The evidence collected during the investigation supported the original
security alert.

The suspicious file identified in the SIEM was associated with a file
hash that received multiple malicious detections from security vendors
through VirusTotal.

The combination of the SIEM alert information and the external threat
intelligence results provided sufficient evidence to classify the
activity as malicious.

The alert was therefore determined to be a **True Positive**.

---

## 6. Final Verdict

**Verdict: TRUE POSITIVE**

The alert was classified as a true positive following investigation and
threat intelligence validation.

An analyst comment was added to document the investigation outcome and
the alert was subsequently closed.

### Final Verdict

<img width="875" height="602" alt="Screenshot 2026-07-28 100216" src="https://github.com/user-attachments/assets/62cde7c5-cc6c-4c2b-bc9b-df2a71f7d9bd" />


---

## 7. Video Demonstration

The following screen recording demonstrates the SOC L1 alert triage
process, including the investigation of the alert and the final
true-positive verdict.

### SOC L1 True Positive Alert Triage

https://github.com/user-attachments/assets/bec9cf1e-f3cf-4cf6-aab5-e9c8dcd345b0


---

## 8. SOC L1 Skills Demonstrated

This investigation demonstrates practical experience with:

- SOC L1 alert triage
- SIEM alert investigation
- Security event analysis
- Indicator of Compromise identification
- File hash analysis
- Threat intelligence enrichment
- VirusTotal investigation
- Malware identification
- True-positive classification
- Evidence-based decision making
- Analyst documentation
- Alert closure

---

## 9. Investigation Workflow

```text
Alert Received
      ↓
Review Alert & Severity
      ↓
Investigate Alert Details
      ↓
Identify File Hash
      ↓
Extract IoC
      ↓
VirusTotal Threat Intelligence Lookup
      ↓
Review Security Vendor Detections
      ↓
Assess & Correlate Evidence
      ↓
True Positive Verdict
      ↓
Document Findings
      ↓
Close Alert
```

## 10. Key Learning Outcomes

This investigation helped develop practical experience in the SOC L1
alert triage process.

In particular, I practised investigating SIEM alerts, identifying
Indicators of Compromise, performing hash-based threat intelligence
lookups, validating suspicious activity using external intelligence,
and making an evidence-based alert verdict.

The investigation also reinforced the importance of using multiple
sources of evidence when determining whether an alert represents a
genuine security incident.

## Disclaimer

This investigation was completed in the TryHackMe training environment
for educational and portfolio purposes.
