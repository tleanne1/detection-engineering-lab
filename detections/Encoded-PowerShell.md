# Encoded PowerShell Detection

## Objective

Identify PowerShell commands executed using Base64 encoded payloads.

---

## Threat

Attackers commonly use encoded PowerShell commands to conceal malicious activity and evade traditional security controls.

---

## MITRE ATT&CK

| Technique | ID |
|------------|------------|
| PowerShell | T1059.001 |

---

## Data Sources

- DeviceProcessEvents
- DeviceEvents

---

## Detection Logic

Search for PowerShell processes launched using:

- `-enc`
- `-encodedcommand`

---

## Investigation Steps

1. Identify executing user
2. Review parent process
3. Decode payload if possible
4. Review network connections
5. Identify persistence mechanisms

---

## Response Actions

- Isolate endpoint if malicious
- Collect forensic evidence
- Block indicators
- Review additional affected hosts
