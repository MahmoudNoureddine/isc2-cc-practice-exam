# Domain 3: Access Control Concepts — Study Notes
*(~22% of the ISC2 CC exam)*

## 1. AAA Framework — the backbone of access control

| Step | Question it answers | Example |
|---|---|---|
| **Authentication** | "Who are you?" | Entering username + password |
| **Authorization** | "What are you allowed to do?" | System checks if you can open the payroll app |
| **Accounting** | "What did you actually do?" | Logs recording your login time and actions |

> Authentication happens **first**, authorization **second** — you must prove identity before permissions are checked.

## 2. Authentication Factors ("something you...")

| Factor | Category | Examples |
|---|---|---|
| Something you **know** | Knowledge | Password, PIN, security question |
| Something you **have** | Possession | Smart card, USB security key, phone (OTP app) |
| Something you **are** | Inherence | Fingerprint, retina scan, facial recognition |
| Something you **do** | Behavior (less common) | Typing rhythm, gait analysis |
| Somewhere you **are** | Location | GPS/IP-based geofencing |

- **MFA (Multi-Factor Authentication)** = 2+ factors from *different* categories. Two passwords = still single-factor (both "something you know")!
- **False Rejection (False Negative)** — biometric wrongly denies a legitimate user.
- **False Acceptance (False Positive)** — biometric wrongly grants an unauthorized person. **False acceptance is the more dangerous failure mode.**

## 3. Access Control Models — the classic exam favorite

| Model | Who sets permissions? | Key trait | Typical use |
|---|---|---|---|
| **DAC** (Discretionary) | The resource **owner** | Flexible, owner decides | Shared drives, personal files |
| **MAC** (Mandatory) | Central authority (system-enforced labels/clearances) | Rigid, users can't override | Military/government classified systems |
| **RBAC** (Role-Based) | Access tied to **job role** | Scales well in organizations | Corporate systems, EHR by job title |
| **ABAC** (Attribute-Based) | Access decided by **multiple attributes** (user, resource, environment) combined | Dynamic, context-aware | Cloud apps, conditional access |
| **Rule-Based** | Predefined **if-then rules** applied to everyone | Static, uniform logic | Firewall rules, ACLs |

> Quick trigger words on the exam:
> - "Owner decides" → **DAC**
> - "Clearance level / classification label, can't be changed by user" → **MAC**
> - "Based on job title/department" → **RBAC**
> - "Multiple conditions combined (device + time + location)" → **ABAC**
> - "If X then Y, applies to all" → **Rule-Based**

## 4. Identity Lifecycle

- **Provisioning** — creating an account and granting appropriate initial access (new hire/onboarding).
- **Recertification (access review)** — periodically verifying access is still appropriate (e.g., quarterly manager review) — prevents "privilege creep."
- **Deprovisioning** — removing/disabling access, typically at termination or role change. **Forgetting this step is one of the most commonly tested failure scenarios.**

## 5. Privileged & Federated Access

- **Privileged Access Management (PAM)** — controls, vaults, rotates, and monitors credentials for high-risk accounts (domain admin, root).
- **Just-in-Time (JIT) access** — elevated privileges granted only for a limited time window, then auto-revoked.
- **Single Sign-On (SSO)** — authenticate once, access multiple systems **within the same organization/trust domain**.
- **Federation** — identity trust extended **across separate organizations** (e.g., university login works on a partner library site).

> SSO = one login, multiple apps, *same org*. Federation = one identity, *across orgs*.

## 6. Centralized Authentication Protocols

| Protocol | Key trait |
|---|---|
| **RADIUS** | Centralized AAA, commonly UDP, used for network/VPN/Wi-Fi access |
| **TACACS+** | Similar to RADIUS, often used for network device admin access, TCP-based |
| **Kerberos** | Uses time-stamped **tickets** issued by a **Key Distribution Center (KDC)** — common in Windows AD environments |
| **LDAP** | Directory service protocol for looking up/managing users, groups, resources |
| **SAML/OAuth** | Used for federation and web/SSO authentication |

## 7. Physical Access Control

- **Badge readers, locks, fences, guards** — physical controls restricting entry.
- **Mantrap** — two interlocking doors; the second won't open until the first closes and identity is verified. Prevents tailgating.
- **Tailgating/Piggybacking** — an unauthorized person follows an authorized person through a secured door.
- **Visitor management** — sign-in, temporary badges, escort requirements.

## 8. Supporting Concepts

- **Access Control List (ACL)** — a list attached to an object (file/folder/network) specifying which subjects have which permissions.
- **Least privilege & need-to-know** apply here too — access models should be configured to enforce both.
- **Compensating control** — used when the ideal access control can't be applied (e.g., legacy system can't support MFA → isolate it on a segmented network with heavy monitoring instead).
- **Honeypot** — a deliberately vulnerable decoy system used to lure and study attackers (not really "access control" but often grouped here in scenario questions about unauthorized access).

## Fast-Recall Summary
- AAA = Authenticate → Authorize → Account (in that order).
- Factors: know / have / are / do / location — MFA needs 2+ *different* categories.
- Models: DAC (owner), MAC (central/labels), RBAC (role), ABAC (attributes), Rule-Based (if-then).
- Provisioning → Recertification → Deprovisioning — deprovisioning failures are a classic exam scenario.
- SSO = same org. Federation = across orgs.
- Kerberos = tickets + KDC. RADIUS = network AAA. LDAP = directory lookups.
- Mantrap defeats tailgating.
