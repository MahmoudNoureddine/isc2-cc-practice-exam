# Domain 1: Security Principles — Study Notes
*(~26% of the ISC2 CC exam)*

## 1. The CIA Triad

| Principle | Definition | Broken by... | Protected by... |
|---|---|---|---|
| **Confidentiality** | Only authorized people/systems can view data | Data breach, eavesdropping, shoulder surfing | Encryption, access control, classification |
| **Integrity** | Data is accurate and unaltered | Tampering, man-in-the-middle edits, corruption | Hashing, checksums, digital signatures, version control |
| **Availability** | Authorized users can access data/systems when needed | DoS/DDoS, hardware failure, natural disaster | Redundancy, backups, load balancing, patching |

**Related concepts (often tested alongside CIA):**
- **Non-repudiation** — a party cannot deny having performed an action (achieved via digital signatures, logs). Not one of the three CIA pillars, but closely related to integrity + accountability.
- **Authenticity** — assurance that data/communication genuinely comes from the claimed source.

## 2. Risk Terminology

- **Asset** — anything of value to the organization (data, systems, people, reputation).
- **Threat** — anything with the potential to cause harm (e.g., hacker, malware, fire, insider).
- **Vulnerability** — a weakness that could be exploited (e.g., unpatched software, weak password policy).
- **Risk** = likelihood × impact of a threat exploiting a vulnerability.
- **Exposure** — the extent to which an asset is susceptible to loss from a threat.
- **Threat actor** — the entity carrying out the threat (nation-state, insider, hacktivist, script kiddie).

> Quick memory trick: **Threat exploits a Vulnerability, creating Risk to an Asset.**

## 3. Risk Treatment (4 strategies)

| Strategy | What it means | Example |
|---|---|---|
| **Avoidance** | Eliminate the activity causing the risk | Discontinue a risky product line |
| **Mitigation** | Reduce likelihood/impact with controls | Deploy firewall, MFA, encryption |
| **Transfer** | Shift impact to a third party | Cyber insurance, outsourcing |
| **Acceptance** | Acknowledge and do nothing further (cost of fixing > benefit) | Live with a low-impact, low-cost risk |

**Other key risk terms:**
- **Inherent risk** — risk level before any controls are applied.
- **Residual risk** — risk that remains *after* controls are applied.
- **Risk appetite** — how much risk an organization is willing to accept overall.
- **Risk tolerance** — acceptable variation around that appetite for a specific risk.

## 4. Control Categories (memorize both axes)

**By type (how it works):**
- **Technical/Logical** — firewalls, encryption, IDS/IPS, access control software
- **Administrative/Managerial** — policies, training, background checks, procedures
- **Physical** — locks, fences, guards, badge readers, mantraps

**By function (what it does):**
- **Preventive** — stops an incident before it happens (firewall, lock, MFA)
- **Detective** — identifies that something happened (IDS, CCTV footage review, audit log)
- **Corrective** — restores/fixes after an incident (restore from backup, patch)
- **Deterrent** — discourages an attempt (warning signs, visible cameras, lighting)
- **Compensating** — an alternative control when the primary one can't be used (extra monitoring instead of patching a legacy system)

> A control can belong to one type *and* one function at the same time — e.g., a firewall is **technical + preventive**; a security guard is **physical + preventive/deterrent**.

## 5. Governance & Document Hierarchy

Order from most general/mandatory to most specific:

1. **Policy** — high-level, mandatory statement of management intent ("All data must be protected").
2. **Standard** — specific, mandatory requirements supporting a policy ("Passwords must be 14+ characters").
3. **Procedure** — detailed step-by-step instructions ("How to reset a password").
4. **Guideline** — recommended, *not* mandatory, best practices.
5. **Baseline** — the minimum security configuration required for a system type.

## 6. Foundational Security Principles

- **Least privilege** — give users only the access needed to do their job, nothing more.
- **Need to know** — restrict access to specific info required for a task, even if cleared for more.
- **Separation of duties (SoD)** — split critical tasks between multiple people to prevent fraud/error (e.g., one person requests a payment, another approves it).
- **Dual control** — two people must act *together* to complete one sensitive action (e.g., two keys to open a vault).
- **Job rotation** — periodically moving staff between roles to surface fraud/errors and reduce single points of failure.
- **Mandatory vacation** — forcing time off so someone else can review the employee's work.
- **Defense in depth** — layering multiple different controls so no single point of failure compromises the whole system.

## 7. Laws, Regulations & Frameworks (know what each governs)

| Regulation/Standard | Governs |
|---|---|
| **GDPR** | Personal data of EU individuals |
| **HIPAA** | Protected health information (PHI) in the U.S. |
| **PCI DSS** | Payment card / cardholder data |
| **SOX** | Financial reporting integrity (U.S. public companies) |
| **ISO 27001** | International standard for information security management systems (ISMS) |
| **NIST CSF / 800-53** | U.S. cybersecurity framework/control catalog |

## 8. ISC2 Code of Ethics — 4 Canons (in priority order)

1. Protect society, the common good, necessary public trust and confidence, and the infrastructure.
2. Act honorably, honestly, justly, responsibly, and legally.
3. Provide diligent and competent service to principals (employers/clients).
4. Advance and protect the profession.

> If a scenario question pits two canons against each other, **canon 1 (protect society) wins** — it's listed first for a reason.

## Fast-Recall Summary
- CIA = Confidentiality, Integrity, Availability — know which attack breaks which.
- Risk = Threat × Vulnerability → treated via Avoid/Mitigate/Transfer/Accept.
- Controls = Type (Technical/Admin/Physical) × Function (Preventive/Detective/Corrective/Deterrent/Compensating).
- Policy → Standard → Procedure → Guideline (mandatory to optional).
- Least privilege ≠ Need to know ≠ Separation of duties — know the difference.
- Code of Ethics: society first, always.
