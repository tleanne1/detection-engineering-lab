# ⚡ Detection Engineering Lab

Enterprise Detection Engineering Lab focused on developing, tuning, validating, and documenting security detections using Microsoft Defender, Microsoft Sentinel, KQL, and MITRE ATT&CK.

---

## Overview

This project demonstrates practical detection engineering workflows used to identify malicious activity, reduce false positives, improve alert fidelity, and support threat hunting operations.

The lab focuses on:

- Custom Detection Development
- Detection Tuning
- KQL Analytics
- MITRE ATT&CK Mapping
- Detection Validation
- Threat Hunting Support
- Incident Response Enablement

---

## Technologies

- Microsoft Defender for Endpoint
- Microsoft Sentinel
- Azure Log Analytics
- Kusto Query Language (KQL)
- MITRE ATT&CK Framework

---

## Detection Coverage

| Detection | ATT&CK Technique |
|------------|------------------|
| Encoded PowerShell Execution | T1059.001 |
| Suspicious PowerShell Download | T1059.001 |
| Registry Persistence | T1547.001 |
| Credential Dumping Indicators | T1003 |
| Remote Service Creation | T1021 |
| Lateral Movement Activity | T1021 |
| Suspicious Scheduled Tasks | T1053 |
| Abnormal Authentication Activity | T1078 |

---

## Detection Lifecycle

1. Threat Research
2. Detection Design
3. KQL Development
4. Testing & Validation
5. False Positive Analysis
6. Tuning
7. Deployment
8. Continuous Improvement

---

## MITRE ATT&CK Alignment

The detections within this repository are mapped to MITRE ATT&CK techniques to improve coverage visibility and detection maturity.

---

## Repository Structure

```text
detection-engineering-lab
│
├── README.md
│
├── detections
│   ├── Encoded-PowerShell.md
│   ├── Registry-Persistence.md
│   ├── Credential-Dumping.md
│   ├── Lateral-Movement.md
│   └── Scheduled-Task-Persistence.md
│
├── kql
│   ├── encoded-powershell.kql
│   ├── registry-persistence.kql
│   ├── credential-dumping.kql
│   ├── lateral-movement.kql
│   └── scheduled-task.kql
│
├── mitre-mapping
│   └── ATTACK-Mapping.md
│
├── validation
│   └── Detection-Validation-Guide.md
│
└── screenshots
```

---

## Detection Engineering Workflow

![Detection Lifecycle](screenshots/Detection-Lifecycle.png)

Threat Research → Detection Design → KQL Development → Validation → Tuning → Deployment → Continuous Improvement

---

## ATT&CK Coverage

![MITRE Coverage](screenshots/MITRE-Mapping.png)

---

## Author

Tracey Buentello

Security Engineer | AI Security | SOC Automation | Threat Detection
