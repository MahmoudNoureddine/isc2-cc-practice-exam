# Domain 5: Security Operations — Study Notes
*(~18% of the ISC2 CC exam)*

## 1. Data Classification & Data States

**Classification levels (typical private-sector scheme, low → high sensitivity):**
Public → Internal Use Only → Confidential → Restricted/Top Secret

- Higher classification = stricter handling, encryption, and access requirements.

**Data states — know which protection applies to which:**

| State | Definition | Primary protection |
|---|---|---|
| **Data at rest** | Stored on disk/database/media | Encryption (AES-256), access controls |
| **Data in transit** | Actively moving across a network | TLS/SSL, VPN, IPSec |
| **Data in use** | Actively being processed in memory | Secure enclaves, memory encryption |

## 2. Data Loss Prevention (DLP)

- Monitors and **blocks unauthorized transmission** of sensitive data (email attachments, USB transfers, uploads).
- Often tied to data classification — DLP rules trigger based on data labeled "Confidential" or matching patterns (like credit card numbers).

## 3. Asset Management

- Maintaining an accurate **inventory** of hardware, software, and data assets.
- **You can't secure what you don't know exists** — unmanaged/unknown ("shadow IT") assets are a common root cause in breach scenarios.
- Supports patching, monitoring, and vulnerability management.

## 4. Configuration & Change Management

- **Change management** — formal process to review, test, approve, and document changes before deployment (prevents unplanned outages from unreviewed changes).
- **Security baseline** — documented minimum required secure configuration for a system type before it goes into production.
- Deploying changes/patches directly to production **without testing** is a classic exam red flag.

## 5. Patch & Vulnerability Management

| Term | Definition |
|---|---|
| **Vulnerability scanning** | **Passive/automated** identification of known weaknesses (missing patches, misconfigurations) — does NOT exploit them |
| **Penetration testing** | **Active** attempt to exploit identified weaknesses to prove real-world impact — done by ethical hackers |
| **Patch management** | The full cycle: identify → test (non-production first!) → deploy updates that fix vulnerabilities |
| **Risk-based prioritization** | Fixing vulnerabilities based on exploitability, exposure (internet-facing?), and severity — not randomly |

> Vulnerability scan = "Is the door unlocked?" Penetration test = "Let's actually try to open it and see what's behind it."

## 6. Logging & Monitoring

- **Logging** — recording system/user activity for monitoring, troubleshooting, and forensic investigation.
- **SIEM (Security Information and Event Management)** — aggregates and **correlates** logs from many sources to detect patterns/anomalies and generate alerts (e.g., failed logins from multiple countries on one account in a short window).
- **Log retention policy** — logs must be kept long enough to support investigations discovered after the fact (too-short retention = common audit finding).

## 7. Malware Defense

- **Antivirus/anti-malware** — detects, quarantines, and removes known malicious software.
- **Sandboxing** — safely detonates/executes suspicious files in an isolated environment to observe behavior without risking production systems.
- **Threat intelligence** — external feeds of known malicious IPs/domains/indicators used to proactively block threats.

## 8. Backup Strategies (also relevant to Domain 2)

| Type | Captures | Restore needs |
|---|---|---|
| **Full** | Everything | Just the one full backup |
| **Incremental** | Changes since **last backup of any kind** | Full + every incremental since |
| **Differential** | Changes since **last full backup** | Full + latest differential only |

- **3-2-1 rule**: 3 copies, 2 media types, 1 offsite.
- **Test restores regularly** — an unverified backup may be corrupted or incomplete.

## 9. Secure Disposal

- **Media sanitization** — securely wiping or physically destroying storage media before disposal/recycling, so data can't be recovered.
- **Data retention policy** — defines how long data is kept and requires **secure destruction** (not just deletion) once the retention period ends.

## 10. Security Awareness & Social Engineering

- **Security awareness training** — reduces human-related risk (phishing, pretexting) through education and simulated phishing tests.
- **Social engineering** — manipulating people (urgency, authority, impersonation) to bypass normal security procedures. Common forms:
  - **Phishing** — fraudulent emails
  - **Pretexting** — fabricated scenario/impersonation (e.g., fake CEO call)
  - **Tailgating** — physical follow-through a secured door (see Domain 3)
  - **Business Email Compromise (BEC)** — impersonating an executive to request a wire transfer

## 11. Auditing

- **Security audit** — independent review of logs, configurations, and policy compliance; produces findings/gaps for remediation.
- Different from a vulnerability scan or pen test — an audit checks **compliance with policy/standards**, not just technical weaknesses.

## 12. Operational Metrics & SLAs

- SOCs often define **SLAs** for incident handling (e.g., "acknowledge critical alerts within 15 minutes, investigate within 1 hour").
- Escalation procedures apply if those timeframes are missed.

## Fast-Recall Summary
- Data states: at rest (encrypt storage), in transit (encrypt network), in use (protect memory).
- DLP blocks unauthorized data movement; asset management ensures nothing is "invisible."
- Change management = test/approve before deploying; security baseline = minimum required config.
- Vulnerability scan = passive find. Pen test = active exploit attempt.
- SIEM = correlate logs across the org for alerting.
- Full/Incremental/Differential backups + 3-2-1 rule + test your restores.
- Media sanitization ≠ simple deletion.
- Security awareness training is the primary defense against social engineering.
