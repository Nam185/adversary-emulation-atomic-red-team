# Adversary Emulation & Detection Validation — Atomic Red Team / MITRE ATT&CK

Reproduced real-world attacker techniques using the open-source **Atomic Red Team**
framework, mapped to the **MITRE ATT&CK** model, to validate detection coverage on a
Windows 10 environment. Course Project I (IT3910E) at HUST — **Grade: A+**.

## Overview
The goal was *purple teaming*: safely execute known attack techniques and measure whether
the system can observe/detect them, then identify blind spots in monitoring and logging.

## Tactics covered (MITRE ATT&CK)
- Credential Access
- Lateral Movement
- Discovery
- Collection
- Command & Control
- Exfiltration
- Impact

## What's in this repo
- `Project1-AtomicRedTeam-Report.pdf` — full report (technique-by-technique walkthrough,
  execution steps, screenshots, and analysis).
- `atomic-test-results.xlsx` — results log: each technique / sub-test with success/fail
  status and environment notes.

## Method
1. Selected atomic tests from Atomic Red Team mapped to specific ATT&CK technique IDs.
2. Executed each test on Windows 10 and recorded the outcome.
3. Logged success/fail and reasons (e.g., OS-specific tests not applicable).
4. Analyzed the success ratio per tactic to estimate detection coverage and gaps.

## Demonstration videos
Recorded executions of the attack techniques (Google Drive):
https://drive.google.com/drive/folders/1yn38jI5qiPxzeodnVWkUaaSyIVK2vRMW

## Tools & environment
Atomic Red Team (Red Canary) · MITRE ATT&CK · PowerShell · Windows 10

## Key takeaway
Atomic Red Team is a repeatable, low-risk way to verify defensive coverage: it surfaces
which attacker techniques go undetected, giving a measurable baseline to improve logging,
detection rules, and incident response.

## Team
Tran Hoai Nam, Tran Trung Hieu · Supervisor: Tran Dinh Kien Giang · 2025

## References
- Red Canary — Atomic Red Team: https://github.com/redcanaryco/atomic-red-team
- MITRE ATT&CK: https://attack.mitre.org/
