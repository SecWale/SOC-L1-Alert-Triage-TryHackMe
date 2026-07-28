# SOC L1 Alert Triage – False Positive Investigation

## Overview

This write-up documents a Security Operations Centre (SOC) Level 1
alert triage investigation completed in the TryHackMe SIEM environment.

The objective was to investigate a security alert, review the available
network and alert information, determine whether the activity represented
genuine malicious behaviour, and assign an appropriate verdict.

**Final Verdict:** False Positive

---

## Investigation Summary

**Environment:** TryHackMe

**Platform:** TryHackMe SIEM

**Investigation Type:** SOC L1 Alert Triage

**Analyst:** Olawale Otasanya

**Alert Classification:** False Positive

**Investigation Status:** Completed

**Final Action:** Alert closed

---

## 1. Alert Overview

The investigation began with a review of the alert queue within the
TryHackMe SIEM.

I reviewed the available alert information, including the alert
description, severity, status and other relevant metadata, to understand
why the activity had been flagged.

### Alert Overview

<img width="1917" height="677" alt="Screenshot 2026-07-28 082428" src="https://github.com/user-attachments/assets/0736188b-5e04-4696-a00f-25150d810cac" />


The alert severity and available context were used to determine the
priority of the investigation and identify the information that required
further analysis.

---

## 2. Investigation

I opened the alert and reviewed the investigation details provided by
the SIEM.

The investigation focused on the available source and destination
information, together with the amount of data transferred between the
systems.

The following information was reviewed:

- Source IP address
- Destination IP address
- Source and destination network information
- Data transferred
- Relevant alert details
- Activity associated with the alert

### Investigation Details

<img width="1917" height="417" alt="Screenshot 2026-07-28 082609" src="https://github.com/user-attachments/assets/0768ec35-2649-49e7-814f-6fb4a4130727" />


Reviewing the source and destination information helped establish the
context of the network activity and determine whether the activity
supported the original alert.

---

## 3. Analysis

After reviewing the available alert and network information, I assessed
the activity as not malicious.

Although the activity had triggered a security alert, the available
evidence did indicate that a Zoom meeting took place, and nothing
malicious was observed.

The alert was therefore determined to be a **False Positive**.

This highlights an important part of SOC L1 alert triage: an alert
should not automatically be treated as a confirmed security incident.
The analyst must review the available evidence and make an
evidence-based decision.

---

## 4. Final Verdict

**Verdict: FALSE POSITIVE**

Following the investigation, the alert was classified as a false
positive.

An analyst comment was added to document the investigation outcome and
the alert was subsequently closed.

### Final Verdict

<img width="856" height="587" alt="Screenshot 2026-07-28 083139" src="https://github.com/user-attachments/assets/5f3ca840-1380-48d0-bdf0-7dc47e981863" />


---

## 5. Video Demonstration

The following screen recording demonstrates the alert triage process,
including the investigation of the alert and the final false-positive
verdict.

### SOC L1 False Positive Alert Triage


https://github.com/user-attachments/assets/a7f231d9-71e3-4a37-aaa3-4845a8430c93





---

## 6. SOC L1 Skills Demonstrated

This investigation demonstrates practical experience with:

- SOC L1 alert triage
- SIEM alert investigation
- Alert severity assessment
- Security event analysis
- Network activity analysis
- Source and destination analysis
- False-positive identification
- Evidence-based decision making
- Analyst documentation
- Alert closure

---

## 7. Investigation Workflow

```text
Alert Received
      ↓
Review Alert & Severity
      ↓
Review Investigation Details
      ↓
Analyse Source
      ↓
Assess Network Activity
      ↓
Determine Alert Classification
      ↓
Document Findings
      ↓
Close Alert
```

## 8. Key Learning Outcomes

This exercise helped develop practical experience in understanding the
SOC L1 alert triage workflow.

In particular, I practised reviewing alerts, investigating associated
network information, assessing whether an alert was supported by
sufficient evidence, and documenting an appropriate verdict.

The investigation also reinforced the importance of distinguishing
between a security alert and a confirmed security incident.

## 9. Disclaimer

This investigation was completed in the TryHackMe training environment
for educational and portfolio purposes.
