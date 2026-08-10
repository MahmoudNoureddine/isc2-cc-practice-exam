# ISC2 Certified in Cybersecurity (CC) — 200 Scenario-Based Practice Questions

All 200 questions below are scenario-based, matching the applied, situational style used on the official ISC2 CC exam. Each includes four options, the correct answer, and a justification. Questions are organized by the five official CC domains, weighted to match the real exam.

| Domain | Questions | Approx. Weight |
|---|---|---|
| 1. Security Principles | 1–52 | 26% |
| 2. Business Continuity, Disaster Recovery & Incident Response Concepts | 53–72 | 10% |
| 3. Access Control Concepts | 73–116 | 22% |
| 4. Network Security | 117–164 | 24% |
| 5. Security Operations | 165–200 | 18% |

---

## Domain 1: Security Principles

**Q1.** A hospital's patient records database goes offline for six hours due to a hardware failure, but no data was altered or disclosed. Which CIA principle was most directly violated?
A) Confidentiality
B) Integrity
C) Availability
D) Non-repudiation

**Answer:** C
**Justification:** Doctors could not access records during the outage; this impacts availability, since the data itself was neither disclosed nor altered.

**Q2.** An attacker intercepts an email between two executives and changes the bank account number in a wire transfer request before forwarding it. Which principle was violated?
A) Confidentiality
B) Integrity
C) Availability
D) Authentication

**Answer:** B
**Justification:** The message content was altered without authorization, which is a violation of integrity, even though confidentiality was also arguably compromised, the alteration is the defining harm here.

**Q3.** A former employee's laptop, containing unencrypted customer records, is stolen from their car. No evidence exists that the data was ever accessed. Which principle is at risk?
A) Availability
B) Confidentiality
C) Integrity
D) Accountability

**Answer:** B
**Justification:** The exposure of sensitive data to a potentially unauthorized party threatens confidentiality, regardless of whether the data was actually viewed.

**Q4.** A company's e-commerce site crashes every Black Friday due to traffic volume, costing significant revenue. The security team recommends load balancers and auto-scaling. This primarily addresses which principle?
A) Confidentiality
B) Integrity
C) Availability
D) Non-repudiation

**Answer:** C
**Justification:** Load balancing and auto-scaling ensure the system remains accessible under high demand, directly supporting availability.

**Q5.** After a contract dispute, a vendor claims they never approved a change order. The organization produces a digitally signed email as proof they did. This is an example of which principle in action?
A) Confidentiality
B) Availability
C) Non-repudiation
D) Least privilege

**Answer:** C
**Justification:** The digital signature prevents the vendor from credibly denying they sent the approval, which is the essence of non-repudiation.

**Q6.** A security analyst discovers that a legacy application still uses default administrator credentials that were never changed since installation. This represents a:
A) Threat
B) Vulnerability
C) Risk
D) Exploit

**Answer:** B
**Justification:** The unchanged default credentials are a weakness in the system that could be exploited — a vulnerability.

**Q7.** A threat intelligence report warns that a specific nation-state group is actively targeting companies in the organization's industry using phishing campaigns. In risk terms, this group represents a:
A) Vulnerability
B) Threat actor
C) Exposure
D) Control

**Answer:** B
**Justification:** The nation-state group is the entity capable of exploiting weaknesses to cause harm, making it a threat actor.

**Q8.** A CISO calculates that a data breach affecting the customer database would likely cost $2 million and has an estimated 10% chance of occurring this year. This calculation is an example of:
A) Vulnerability scanning
B) Risk assessment
C) Penetration testing
D) Change management

**Answer:** B
**Justification:** Estimating the likelihood and potential impact of a threat event is the core activity of risk assessment.

**Q9.** After reviewing risk assessment results, a manufacturing company decides to stop offering an online customer portal because the risk of exposing production system data is too great, even with security controls. This is:
A) Risk mitigation
B) Risk avoidance
C) Risk transfer
D) Risk acceptance

**Answer:** B
**Justification:** Discontinuing the activity entirely to eliminate the associated risk is risk avoidance.

**Q10.** A retailer purchases a cyber liability insurance policy that will reimburse the company up to $5 million in the event of a data breach. This is an example of:
A) Risk mitigation
B) Risk avoidance
C) Risk transfer
D) Risk acceptance

**Answer:** C
**Justification:** Shifting the financial consequences of a risk to an insurer is risk transfer.

**Q11.** A small nonprofit determines that securing an old, rarely used file server would cost more than the value of the data it holds, and decides to leave it as-is while monitoring it lightly. This decision represents:
A) Risk avoidance
B) Risk mitigation
C) Risk acceptance
D) Risk transfer

**Answer:** C
**Justification:** The organization is knowingly living with the risk because the cost of addressing it outweighs the benefit — risk acceptance.

**Q12.** A bank deploys multi-factor authentication, encrypts stored data, and implements intrusion detection after a risk assessment identified account takeover as a top threat. This combination of actions represents:
A) Risk avoidance
B) Risk mitigation
C) Risk transfer
D) Risk acceptance

**Answer:** B
**Justification:** Implementing controls to reduce the likelihood and impact of a risk, without eliminating the underlying activity, is risk mitigation.

**Q13.** After deploying encryption, MFA, and network monitoring, a security team still estimates a 3% annual chance of a successful breach. This remaining risk is called:
A) Inherent risk
B) Residual risk
C) Total risk
D) Risk appetite

**Answer:** B
**Justification:** Residual risk is what remains after controls have been applied to reduce the original (inherent) risk.

**Q14.** A board of directors states that the company is willing to accept minor operational disruptions but will not tolerate any risk that could lead to regulatory fines. This statement reflects the organization's:
A) Risk register
B) Risk appetite
C) Vulnerability assessment
D) Threat model

**Answer:** B
**Justification:** This describes the level and type of risk the organization is willing to accept, which defines its risk appetite.

**Q15.** A company installs badge readers on server room doors, requiring employees to scan a card before entry. What type of control is this?
A) Administrative
B) Technical
C) Physical
D) Corrective

**Answer:** C
**Justification:** Badge readers control physical entry to a facility or room, making them a physical control (even though they use technology, their function is physical access restriction).

**Q16.** After a phishing incident, an organization requires all staff to complete annual security awareness training. What type of control is this?
A) Physical
B) Technical
C) Administrative
D) Detective

**Answer:** C
**Justification:** Training and policy-driven initiatives that shape employee behavior are administrative controls.

**Q17.** A network engineer configures a firewall to block all inbound traffic on port 3389 (RDP) from the internet. What type of control has been implemented?
A) Administrative, preventive
B) Technical, preventive
C) Physical, detective
D) Technical, corrective

**Answer:** B
**Justification:** The firewall is a technology-based control that stops unauthorized traffic before it reaches internal systems, making it a technical, preventive control.

**Q18.** A SOC analyst notices repeated failed login attempts on a critical server through SIEM alerts and immediately investigates. Which type of control detected this activity?
A) Preventive
B) Detective
C) Corrective
D) Deterrent

**Answer:** B
**Justification:** The SIEM alert identified suspicious activity after it began occurring, which is the function of a detective control.

**Q19.** Following a ransomware attack, the IT team restores all affected servers from clean backups taken the night before. This action is an example of a:
A) Preventive control
B) Detective control
C) Corrective control
D) Deterrent control

**Answer:** C
**Justification:** Restoring systems to a known-good state after an incident is a corrective control, aimed at recovery.

**Q20.** A retail store posts large signs stating "24-Hour Video Surveillance in Effect" near its entrances, even though the cameras are not always monitored live. The primary purpose of these signs is:
A) Preventive
B) Deterrent
C) Detective
D) Corrective

**Answer:** B
**Justification:** The signage is intended to discourage potential wrongdoers from attempting theft or intrusion, making it a deterrent control.

**Q21.** A company cannot immediately patch a critical legacy system due to compatibility issues with a manufacturing line, so it isolates the system on a segmented VLAN with restricted access and enhanced monitoring instead. This is an example of a:
A) Preventive control
B) Deterrent control
C) Compensating control
D) Corrective control

**Answer:** C
**Justification:** When the ideal control (patching) cannot be applied, an alternative safeguard achieving a similar risk-reduction goal is a compensating control.

**Q22.** During a penetration test, a security consultant discovers a critical vulnerability but decides to disclose it responsibly to the client rather than sell it on the dark web. This decision best reflects which ISC2 Code of Ethics canon?
A) Advance and protect the profession
B) Act honorably, honestly, justly, responsibly, and legally
C) Provide diligent and competent service to principals
D) Protect society, the common good, necessary public trust and confidence, and the infrastructure

**Answer:** D
**Justification:** Choosing not to exploit or sell the vulnerability protects the broader public trust and infrastructure, aligning with the first and most fundamental canon of the Code of Ethics.

**Q23.** An ISC2 member discovers that a colleague is exaggerating their credentials on LinkedIn to win client contracts. According to the Code of Ethics, what consideration is most relevant here?
A) This is a personal matter and outside the Code's scope
B) Advancing and protecting the profession requires discouraging unqualified practice and misrepresentation
C) The member should ignore it since it doesn't involve a client directly
D) Only law enforcement can address this issue

**Answer:** B
**Justification:** The Code of Ethics canon to "advance and protect the profession" includes discouraging unnecessary or unqualified practice and misrepresentation of credentials.

**Q24.** A junior IT administrator is granted full domain administrator rights simply because it is "easier" than configuring specific permissions for their helpdesk tasks. Which principle is being violated?
A) Separation of duties
B) Least privilege
C) Defense in depth
D) Non-repudiation

**Answer:** B
**Justification:** The administrator has far more access than needed for helpdesk duties, violating least privilege, which requires granting only the minimum access necessary.

**Q25.** A company's accounts payable clerk can both create new vendor records and approve payments to those vendors without any second review. A fraud investigation later reveals this clerk created a fake vendor and paid themselves. Which control failure enabled this?
A) Lack of least privilege
B) Lack of separation of duties
C) Lack of defense in depth
D) Lack of non-repudiation

**Answer:** B
**Justification:** Allowing one person to both create vendors and approve payments without independent oversight is a separation of duties failure, enabling fraud.

**Q26.** A data center requires that two authorized engineers must simultaneously insert and turn separate keys to access the core network room. This design demonstrates:
A) Least privilege
B) Dual control
C) Job rotation
D) Mandatory vacation

**Answer:** B
**Justification:** Requiring two individuals to act together to complete a sensitive action is dual control, reducing the risk of unilateral misuse.

**Q27.** A financial analyst with top-secret clearance requests access to a classified merger document unrelated to their current project. The request is denied. Which principle justifies this denial?
A) Least privilege
B) Need to know
C) Separation of duties
D) Mandatory access control only

**Answer:** B
**Justification:** Even with sufficient clearance, access is restricted to information required for the current task under the need-to-know principle.

**Q28.** An organization rotates its database administrators between the production and reporting teams every six months, partly to reduce single points of knowledge and to help surface any irregularities in prior work. This practice is:
A) Job rotation
B) Mandatory vacation
C) Separation of duties
D) Least privilege

**Answer:** A
**Justification:** Moving staff between roles periodically to reduce dependency on one individual and reveal potential issues is job rotation.

**Q29.** A bank requires all traders to take at least five consecutive business days of vacation each year, during which their trades are reviewed by another employee. This policy is designed to:
A) Enforce least privilege
B) Enable detection of fraud through mandatory vacation
C) Rotate job duties permanently
D) Enforce dual control

**Answer:** B
**Justification:** Mandatory vacation policies force an employee's absence so others can review their work, helping surface fraudulent activity they might otherwise conceal.

**Q30.** A hospital protects patient data using building access badges, encrypted databases, firewalls, endpoint antivirus, and staff training simultaneously, so that if one layer fails, others still provide protection. This strategy is known as:
A) Least privilege
B) Defense in depth
C) Risk transfer
D) Single point of failure elimination

**Answer:** B
**Justification:** Layering multiple, different types of controls so that the failure of one does not result in total compromise is defense in depth.

**Q31.** A new CISO is establishing a framework of roles, responsibilities, and policies to ensure the board of directors has oversight of the company's cybersecurity posture. This work primarily falls under:
A) Incident response
B) Governance
C) Vulnerability management
D) Business continuity

**Answer:** B
**Justification:** Establishing accountability structures, policies, and oversight mechanisms for security is the function of governance.

**Q32.** The executive team issues a high-level, mandatory statement that "all customer data must be protected in accordance with applicable privacy laws," without specifying technical details. This document is best classified as a:
A) Procedure
B) Guideline
C) Policy
D) Standard

**Answer:** C
**Justification:** A brief, high-level, mandatory statement of management intent is a policy; the details are left to supporting standards and procedures.

**Q33.** To support the company's password policy, the IT department publishes a document stating passwords must be a minimum of 14 characters, include three character types, and be changed every 90 days. This document is a:
A) Guideline
B) Standard
C) Procedure
D) Policy

**Answer:** B
**Justification:** Specific, mandatory technical requirements that support a broader policy are documented as standards.

**Q34.** A systems administrator follows a documented, numbered list of exact steps to decommission a server, including which cables to disconnect and which commands to run. This document is a:
A) Policy
B) Standard
C) Guideline
D) Procedure

**Answer:** D
**Justification:** Detailed, step-by-step instructions for performing a specific task are procedures.

**Q35.** A security team publishes recommended (but optional) best practices for securing personal home Wi-Fi networks for remote employees. This is an example of a:
A) Guideline
B) Standard
C) Policy
D) Baseline

**Answer:** A
**Justification:** Recommended, non-mandatory advice is classified as a guideline.

**Q36.** A U.S. software company that processes payment data for customers in Germany and France must comply with strict rules on how it collects, stores, and transfers EU citizens' personal data. Which regulation applies?
A) HIPAA
B) GDPR
C) SOX
D) FISMA

**Answer:** B
**Justification:** GDPR governs the processing of personal data belonging to individuals in the EU, regardless of where the processing company is located.

**Q37.** A clinic's billing system is breached, exposing patients' diagnoses and treatment histories. Which U.S. regulation is most directly relevant to this incident?
A) GDPR
B) HIPAA
C) PCI DSS
D) COPPA

**Answer:** B
**Justification:** HIPAA governs the protection of protected health information (PHI) in the United States, making it directly applicable to this breach.

**Q38.** An online retailer that accepts Visa and Mastercard payments is undergoing an annual assessment to verify it properly encrypts and segments its cardholder data environment. Which standard governs this assessment?
A) ISO 27001
B) PCI DSS
C) NIST CSF
D) SOC 2

**Answer:** B
**Justification:** PCI DSS specifically applies to organizations that store, process, or transmit payment card data.

**Q39.** A newly certified cybersecurity professional is offered a bribe by a competitor to leak their employer's proprietary security architecture. Refusing this offer is most directly guided by which of the following?
A) The company's incident response plan
B) The ISC2 Code of Ethics
C) The organization's disaster recovery plan
D) The vulnerability management policy

**Answer:** B
**Justification:** Ethical obligations to act honorably and protect one's principal's interests, as outlined in the Code of Ethics, directly govern this situation.

**Q40.** A company experiences a breach because an employee reused their corporate password on a personal website that was later compromised. Which principle, if enforced, would have most reduced this risk?
A) Separation of duties
B) Unique, non-reused credentials combined with MFA
C) Job rotation
D) Mandatory vacation

**Answer:** B
**Justification:** Credential reuse is a common attack vector; unique passwords per system and MFA reduce the impact of a password being compromised elsewhere.

**Q41.** During an audit, it is discovered that an IT manager approved their own purchase requests for new security hardware without any secondary review, and the equipment was never actually delivered. What principle would have prevented this?
A) Least privilege
B) Separation of duties
C) Defense in depth
D) Risk transfer

**Answer:** B
**Justification:** Requiring a separate individual to approve purchases would have provided the oversight needed to catch or prevent this fraud.

**Q42.** A security awareness poster campaign reminds employees to lock their workstations when stepping away, in addition to automatic screen lock policies enforced by group policy. Together, these represent which strategy?
A) Risk transfer
B) Defense in depth (administrative + technical layering)
C) Risk avoidance
D) Non-repudiation

**Answer:** B
**Justification:** Combining human-focused administrative controls (posters/training) with technical enforcement (auto-lock) layers different control types — defense in depth.

**Q43.** A company assesses that a competitor is unlikely to conduct industrial espionage against them due to their small market share, and chooses not to invest further in counter-espionage measures. This reflects which risk concept?
A) Risk transfer
B) Risk appetite/acceptance based on threat likelihood
C) Risk avoidance
D) Vulnerability remediation

**Answer:** B
**Justification:** The organization is accepting the (low) risk based on its assessment of threat likelihood, consistent with its risk appetite.

**Q44.** An organization's security policy states, "All laptops must be encrypted," while a companion document specifies "Use AES-256 full-disk encryption enabled via BitLocker," and a third document walks staff through enabling BitLocker step by step. These three documents represent, respectively:
A) Standard, procedure, policy
B) Policy, standard, procedure
C) Procedure, policy, standard
D) Guideline, policy, standard

**Answer:** B
**Justification:** The mandatory high-level statement is the policy, the specific mandatory technical requirement is the standard, and the step-by-step instructions are the procedure.

**Q45.** A manufacturing plant installs motion-activated lighting and fencing around its perimeter specifically to discourage trespassers before they attempt to breach the facility. This is best classified as a:
A) Preventive, physical control
B) Deterrent, physical control
C) Detective, technical control
D) Corrective, administrative control

**Answer:** B
**Justification:** The lighting and fencing are intended to discourage (deter) potential intruders from attempting entry, making this a deterrent physical control.

**Q46.** A company's incident response retrospective reveals that a breach could have been avoided if a vendor's remote access account had been disabled after their contract ended six months earlier. Which control failure is most directly implicated?
A) Failure of least privilege
B) Failure of deprovisioning/account lifecycle management
C) Failure of dual control
D) Failure of risk transfer

**Answer:** B
**Justification:** The vendor's access should have been revoked (deprovisioned) once no longer needed; failing to do so left an unnecessary, exploitable account active.

**Q47.** A CISO presents a risk register to the board showing that ransomware is the top-rated risk based on likelihood and potential financial impact. The board approves budget for additional endpoint detection tools. This entire process illustrates:
A) Incident response
B) Risk assessment leading to risk mitigation
C) Business continuity planning
D) Disaster recovery testing

**Answer:** B
**Justification:** Identifying and rating a risk (assessment) followed by implementing controls to reduce it (mitigation) is exactly this process.

**Q48.** An organization's ethics hotline receives a report that a security engineer is using company scanning tools to test personal side projects without authorization. Which ethical canon is most relevant to evaluating the engineer's conduct?
A) Protect society, the common good, and the infrastructure
B) Provide diligent and competent service to principals
C) Advance and protect the profession
D) Act honorably, honestly, justly, responsibly, and legally toward principals

**Answer:** D
**Justification:** Misusing employer resources for personal purposes without authorization violates the obligation to act honorably, honestly, and responsibly toward one's employer (principal).

**Q49.** A security team implements encryption for data at rest, TLS for data in transit, and strict access controls, all in support of protecting sensitive customer records from disclosure. These controls collectively support which CIA principle primarily?
A) Availability
B) Confidentiality
C) Integrity
D) Non-repudiation

**Answer:** B
**Justification:** Encryption and access controls are primarily aimed at preventing unauthorized disclosure of data, supporting confidentiality.

**Q50.** After a vendor risk assessment reveals that a critical software supplier has poor security practices, the company decides to require the vendor to obtain a specific security certification within 90 days or lose the contract. This is an example of:
A) Risk acceptance
B) Risk mitigation applied to third-party/supply chain risk
C) Risk avoidance
D) Risk transfer

**Answer:** B
**Justification:** Requiring the vendor to improve security practices reduces (mitigates) the risk associated with the third-party relationship rather than eliminating or transferring it.

**Q51.** A company assigns a "data owner" for its HR database who is accountable for determining who may access it, while IT implements the technical access controls. This division of responsibility illustrates:
A) Separation of duties combined with defined governance roles
B) Risk transfer
C) Job rotation
D) Mandatory access control exclusively

**Answer:** A
**Justification:** Distinguishing between who decides access (data owner) and who implements it (IT) is a governance-driven separation of responsibilities.

**Q52.** During onboarding, a new employee is told that violating the company's acceptable use policy could result in termination and potential legal action, and is asked to sign an acknowledgment form. This process primarily supports which control type?
A) Technical, preventive
B) Administrative, preventive/deterrent
C) Physical, detective
D) Technical, corrective

**Answer:** B
**Justification:** Policy acknowledgment and stated consequences are administrative controls that aim to prevent and deter policy violations through employee awareness and accountability.

---

## Domain 2: Business Continuity, Disaster Recovery & Incident Response Concepts

**Q53.** A regional bank's data center floods during a hurricane, taking down all core banking systems. The bank's plan for keeping ATMs, online banking, and branch operations running during this crisis is documented in its:
A) Disaster Recovery Plan
B) Business Continuity Plan
C) Incident Response Plan
D) Vulnerability Management Plan

**Answer:** B
**Justification:** The BCP addresses how critical business functions (like banking operations) continue during and after a disruptive event, beyond just IT restoration.

**Q54.** After the same flooding event, the IT team follows a separate document detailing how to rebuild database servers, restore backups, and reconfigure network equipment at a secondary facility. This document is the:
A) Business Continuity Plan
B) Disaster Recovery Plan
C) Business Impact Analysis
D) Communication Plan

**Answer:** B
**Justification:** The DRP focuses specifically on restoring IT infrastructure and systems, which matches the described technical rebuild activities.

**Q55.** A company determines that its order-processing system must be restored within 4 hours of an outage to avoid unacceptable business impact. This 4-hour figure represents the:
A) RPO
B) RTO
C) MTBF
D) SLA

**Answer:** B
**Justification:** The target maximum time to restore a system after disruption is the Recovery Time Objective.

**Q56.** The same company determines it can tolerate losing at most 15 minutes of transaction data if a system fails, meaning backups must occur at least every 15 minutes. This value is the:
A) RTO
B) RPO
C) MTD
D) MTTR

**Answer:** B
**Justification:** The Recovery Point Objective defines the maximum tolerable data loss, measured in time, driving backup frequency requirements.

**Q57.** A business impact analysis reveals that if the payroll system is down for more than 72 hours, the company will face regulatory penalties and severe reputational damage that could threaten its survival. This 72-hour figure is best described as the:
A) RTO
B) RPO
C) Maximum Tolerable Downtime (MTD)
D) SLA

**Answer:** C
**Justification:** MTD represents the absolute maximum time a function can be unavailable before causing unacceptable/catastrophic harm to the organization.

**Q58.** A financial trading firm maintains a fully mirrored, continuously updated backup facility in another city, ready to take over operations within minutes of a primary site failure. This facility is a:
A) Cold site
B) Warm site
C) Hot site
D) Reciprocal site

**Answer:** C
**Justification:** A facility with real-time data replication and near-immediate failover capability is a hot site.

**Q59.** A mid-sized company maintains an empty data center space with power, cooling, and network connectivity already installed, but no servers or data currently present, to reduce ongoing costs while still enabling faster recovery than starting from nothing. This is a:
A) Hot site
B) Warm site
C) Cold site
D) Mutual aid site

**Answer:** C
**Justification:** A space with only basic infrastructure and no pre-installed equipment or data is a cold site, requiring significant setup time before use.

**Q60.** A company maintains a secondary facility with some servers and network equipment already racked and periodically updated with data snapshots, allowing recovery within about 24-48 hours rather than immediately or from scratch. This is a:
A) Hot site
B) Warm site
C) Cold site
D) Hot standby

**Answer:** B
**Justification:** Partial infrastructure and periodically updated data, requiring some additional setup before full operation, describes a warm site.

**Q61.** A SOC analyst notices unusual outbound traffic at 2 AM and, after investigation, confirms that a server has been compromised and is exfiltrating data. Documenting this confirmation and notifying the incident response team represents which phase?
A) Preparation
B) Detection and Analysis
C) Containment
D) Eradication

**Answer:** B
**Justification:** Validating that suspicious activity is indeed a genuine incident and assessing its scope is the Detection and Analysis phase.

**Q62.** Immediately after confirming a server compromise, the incident response team disconnects the affected server from the network to stop further data exfiltration while investigation continues. This action is part of:
A) Detection and Analysis
B) Containment
C) Eradication
D) Lessons Learned

**Answer:** B
**Justification:** Isolating the compromised system to stop further damage, without yet removing the root cause, is containment.

**Q63.** After isolating the compromised server, the team identifies and removes a backdoor the attacker had installed, and patches the vulnerability the attacker originally exploited. This work falls under:
A) Containment
B) Eradication
C) Recovery
D) Preparation

**Answer:** B
**Justification:** Removing the malicious artifact and closing the exploited vulnerability is the core activity of the eradication phase.

**Q64.** Once the backdoor is removed and the vulnerability patched, the team reconnects the server to the network, restores it from a clean backup, and closely monitors it for several days for signs of reinfection. This is the:
A) Containment phase
B) Eradication phase
C) Recovery phase
D) Preparation phase

**Answer:** C
**Justification:** Returning the system to normal operations and monitoring for recurrence is the recovery phase.

**Q65.** Two weeks after the incident is fully resolved, the security team holds a meeting to discuss what indicators were missed, how detection could have been faster, and what new controls should be implemented. This activity is the:
A) Containment phase
B) Eradication phase
C) Post-Incident Activity / Lessons Learned phase
D) Detection and Analysis phase

**Answer:** C
**Justification:** Reviewing the incident after resolution to identify improvements is the Lessons Learned (post-incident activity) phase.

**Q66.** Before any incident occurs, an organization writes its incident response plan, establishes a response team with defined roles, purchases forensic tools, and conducts tabletop exercises. This work all falls under which phase?
A) Preparation
B) Detection and Analysis
C) Containment
D) Recovery

**Answer:** A
**Justification:** Establishing plans, teams, tools, and training before an incident occurs is the Preparation phase of the incident response lifecycle.

**Q67.** A manufacturing company conducts a study identifying that its order-fulfillment process is the most critical function, that it relies on three specific systems and two key vendors, and that an outage exceeding 8 hours would cause severe financial loss. This study is a:
A) Disaster Recovery Plan
B) Business Impact Analysis
C) Vulnerability Assessment
D) Penetration Test

**Answer:** B
**Justification:** Identifying critical functions, dependencies, and quantifying disruption impact is precisely what a Business Impact Analysis accomplishes.

**Q68.** During a wildfire evacuation, an organization's crisis communication team sends updates to employees, customers, and regulators about the status of operations and expected recovery timelines. This communication plan is typically a component of the organization's:
A) Vulnerability management program
B) Business continuity plan
C) Access control policy
D) Patch management process

**Answer:** B
**Justification:** Communication planning during a disruptive event is a standard component of business continuity planning, ensuring stakeholders remain informed.

**Q69.** After a major earthquake destroys a company's primary data center, engineers spend three days configuring new servers, reinstalling software, and restoring the latest backups at an alternate site before operations resume. Which recovery metric was most directly exceeded, given that the target was 24 hours?
A) RPO
B) RTO
C) MTBF
D) SLA

**Answer:** B
**Justification:** Since the actual recovery time (3 days) exceeded the target restoration time (24 hours), the RTO was exceeded.

**Q70.** A company backs up its database every 4 hours. After a system crash, the most recent backup was 3 hours old, resulting in 3 hours of lost transactions — within the company's defined tolerance. This scenario demonstrates that the company met its:
A) RTO
B) RPO
C) MTD
D) BIA

**Answer:** B
**Justification:** The amount of data lost (3 hours) fell within the acceptable threshold defined by the Recovery Point Objective.

**Q71.** During a tabletop exercise simulating a ransomware attack, participants discover that no one on the response team knows who has the authority to decide whether to pay a ransom. This gap should be addressed by updating the organization's:
A) Network diagram
B) Incident response plan (roles and decision-making authority)
C) Data classification policy
D) Vulnerability scanning schedule

**Answer:** B
**Justification:** Clarifying decision-making authority and roles during incidents is a core element that belongs in the incident response plan.

**Q72.** A company's disaster recovery test reveals that backup tapes stored offsite were corrupted and could not be restored, even though backups were being performed on schedule. What should the organization have been doing to catch this issue earlier?
A) Increasing backup frequency
B) Conducting regular restoration/recovery testing of backups
C) Switching to a hot site
D) Extending the RPO

**Answer:** B
**Justification:** Only periodic restoration testing verifies that backups are actually usable; scheduling backups alone does not guarantee they will restore successfully.

---

## Domain 3: Access Control Concepts

**Q73.** A file owner on a shared drive personally decides to grant "read" access to a colleague for a specific folder, without needing IT or a central authority's approval. This access control model is:
A) Mandatory Access Control
B) Discretionary Access Control
C) Role-Based Access Control
D) Attribute-Based Access Control

**Answer:** B
**Justification:** The resource owner independently deciding who gets access is the defining characteristic of DAC.

**Q74.** A defense contractor's classified document management system assigns "Top Secret," "Secret," and "Confidential" labels to files, and users can only access documents at or below their assigned clearance level, as set centrally by security administrators. This is:
A) Discretionary Access Control
B) Mandatory Access Control
C) Role-Based Access Control
D) Rule-Based Access Control

**Answer:** B
**Justification:** Centrally assigned classification labels and clearance levels that users cannot alter themselves is the hallmark of MAC.

**Q75.** A hospital's EHR system automatically grants nurses access to patient vital signs and medication records, while granting billing staff access only to insurance and payment information, based on each employee's assigned job title. This is:
A) Discretionary Access Control
B) Mandatory Access Control
C) Role-Based Access Control
D) Rule-Based Access Control

**Answer:** C
**Justification:** Access determined by predefined job roles (nurse vs. billing staff) is the definition of RBAC.

**Q76.** A cloud application grants access to a financial report only if the requester is in the Finance department, is accessing from a corporate device, and it is currently within business hours — combining multiple conditions dynamically. This is:
A) Discretionary Access Control
B) Mandatory Access Control
C) Role-Based Access Control
D) Attribute-Based Access Control

**Answer:** D
**Justification:** Evaluating multiple attributes (department, device, time) together to make an access decision is characteristic of ABAC.

**Q77.** A corporate firewall is configured with a rule: "If traffic originates from an external IP and targets port 22, deny it." This static if-then logic applied uniformly to all traffic exemplifies:
A) Discretionary Access Control
B) Rule-Based Access Control
C) Mandatory Access Control
D) Role-Based Access Control

**Answer:** B
**Justification:** Predefined rules (if-then logic) applied consistently to all subjects is rule-based access control.

**Q78.** An employee logging into their laptop types a PIN they memorized during onboarding. This authentication factor is:
A) Something you have
B) Something you are
C) Something you know
D) Somewhere you are

**Answer:** C
**Justification:** A memorized PIN is knowledge-based, falling under "something you know."

**Q79.** A contractor is issued a USB security key that must be physically plugged into their laptop to complete login. This factor is:
A) Something you know
B) Something you have
C) Something you are
D) Something you do

**Answer:** B
**Justification:** A physical device that must be possessed is "something you have."

**Q80.** A bank's mobile app requires customers to complete a facial recognition scan before viewing account balances. This factor is:
A) Something you know
B) Something you have
C) Something you are
D) Somewhere you are

**Answer:** C
**Justification:** A facial scan measures a physical, inherent characteristic, categorized as "something you are."

**Q81.** To log into the company VPN, an employee must enter their password and then approve a push notification sent to their registered smartphone. This combination is an example of:
A) Single-factor authentication
B) Two-factor (multi-factor) authentication
C) Single sign-on
D) Federated identity

**Answer:** B
**Justification:** Combining "something you know" (password) with "something you have" (smartphone) constitutes two-factor/multi-factor authentication.

**Q82.** An employee logs into their company portal once in the morning and is then automatically granted access to email, the HR system, and the expense reporting tool without logging in again. This capability is:
A) Multi-factor authentication
B) Single Sign-On (SSO)
C) Role-Based Access Control
D) Federated identity across organizations

**Answer:** B
**Justification:** Authenticating once and gaining access to multiple internal applications without re-authenticating is Single Sign-On.

**Q83.** A university student uses their university credentials to log into a partner online library service operated by a completely separate organization, because the two institutions have established a trust relationship. This is an example of:
A) Single Sign-On within one organization
B) Identity federation
C) Discretionary access control
D) Privileged access management

**Answer:** B
**Justification:** Using one identity across trust-linked but separate organizations is identity federation.

**Q84.** On an employee's first day, HR notifies IT, who then creates the employee's user account, email, and grants access to systems relevant to their new marketing role. This process is called:
A) Deprovisioning
B) Provisioning
C) Recertification
D) Federation

**Answer:** B
**Justification:** Creating accounts and assigning appropriate initial access is provisioning.

**Q85.** When an employee is terminated, the HR system automatically triggers IT to disable the employee's network account, revoke building badge access, and remove them from all distribution lists within one hour. This process is called:
A) Provisioning
B) Deprovisioning
C) Recertification
D) Escalation

**Answer:** B
**Justification:** Removing or disabling access rights when an employee leaves is deprovisioning.

**Q86.** A security team implements a specialized vault solution that stores, rotates, and monitors the credentials used by domain administrator accounts, requiring justification and approval before checkout. This is an example of:
A) Role-Based Access Control
B) Privileged Access Management (PAM)
C) Federated identity
D) Rule-based access control

**Answer:** B
**Justification:** Controlling, storing, and monitoring elevated/administrator credentials is the specific function of PAM.

**Q87.** Every quarter, department managers must review a report listing which of their employees have access to which systems and confirm or revoke access as appropriate. This activity is known as:
A) Provisioning
B) Access recertification (periodic access review)
C) Deprovisioning
D) Federation

**Answer:** B
**Justification:** Periodic manager verification that access remains appropriate is access recertification, supporting least privilege over time.

**Q88.** A cybersecurity team sets up a deliberately vulnerable server, disconnected from production systems, to lure attackers and study their tactics after noticing repeated probing attempts against the network. This server is a:
A) DMZ host
B) Honeypot
C) Jump box
D) Proxy server

**Answer:** B
**Justification:** A deliberately vulnerable decoy system used to attract and study attackers is a honeypot.

**Q89.** Visitors to a corporate headquarters must sign in at a front desk, receive a temporary badge, and be escorted by an employee at all times while in secure areas. This process is an example of:
A) Technical access control
B) Physical access control
C) Rule-based access control only
D) Federated access control

**Answer:** B
**Justification:** Managing physical entry to a facility through sign-in, badges, and escorts is physical access control.

**Q90.** A secure data center entrance consists of two interlocking doors — the second door will not open until the first is fully closed and the individual is verified — specifically to prevent an unauthorized person from slipping in behind an authorized employee. This design is called a:
A) Turnstile
B) Mantrap
C) Bollard
D) Access control vestibule bypass

**Answer:** B
**Justification:** This two-door interlocking design that prevents unauthorized entry alongside an authorized person is a mantrap.

**Q91.** An employee holds the door open for a person behind them carrying boxes, who does not badge in and is not recognized by the employee. This security failure is known as:
A) Shoulder surfing
B) Tailgating
C) Dumpster diving
D) Pretexting

**Answer:** B
**Justification:** An unauthorized person following an authorized person through a secured entry point without their own credentials is tailgating (piggybacking).

**Q92.** A hospital cannot immediately upgrade an aging medical device running an unsupported operating system because doing so would void the manufacturer's warranty and regulatory certification. Instead, the security team places the device on an isolated network segment with strict firewall rules and continuous monitoring. This approach is an example of:
A) Risk avoidance
B) A compensating control
C) Mandatory access control
D) Role-based access control

**Answer:** B
**Justification:** Since the ideal fix (patching/upgrading) isn't possible, an alternative safeguard achieving similar protection is a compensating control.

**Q93.** A multinational corporation allows employees to use their corporate login credentials to access a third-party expense reporting SaaS platform without creating a separate account on that platform. What access control concept enables this?
A) Discretionary access control
B) Identity federation
C) Mandatory access control
D) Rule-based access control

**Answer:** B
**Justification:** Using one trusted identity across separate organizations/systems is identity federation.

**Q94.** A company's access policy states that contractor accounts automatically expire and are disabled 90 days after creation unless explicitly renewed by a manager. This control is an example of:
A) Mandatory access control
B) Time-based access restriction
C) Discretionary access control
D) Rule-based access control only

**Answer:** B
**Justification:** Automatically expiring access after a defined period is a time-based access restriction, reducing the risk of stale, unused accounts.

**Q95.** An HR system's file share has a list attached to the "Salaries" folder specifying that the Finance group can read and write, the Executive group can only read, and everyone else is denied. This list is a(n):
A) Access Control List (ACL)
B) Security baseline
C) Risk register
D) Directory schema

**Answer:** A
**Justification:** A list defining which subjects have which permissions on a specific object is an Access Control List.

**Q96.** A company's wireless network authenticates devices using a centralized server that validates credentials over UDP before granting network access, commonly used with network switches and Wi-Fi controllers. This protocol is most likely:
A) Kerberos
B) RADIUS
C) SAML
D) OAuth

**Answer:** B
**Justification:** RADIUS is a centralized AAA protocol commonly used for network access authentication, typically operating over UDP.

**Q97.** A Windows domain environment issues time-stamped tickets from a centralized Key Distribution Center to authenticate users when they access network resources, without transmitting passwords repeatedly across the network. This authentication protocol is:
A) RADIUS
B) TACACS+
C) Kerberos
D) LDAP

**Answer:** C
**Justification:** Ticket-based authentication via a KDC is the defining characteristic of Kerberos.

**Q98.** An IT administrator queries a centralized directory to look up an employee's department, manager, and group memberships before troubleshooting their account. This directory service is most likely:
A) DHCP
B) LDAP
C) DNS
D) SNMP

**Answer:** B
**Justification:** LDAP is used to query and manage directory information about users, groups, and resources.

**Q99.** During an incident investigation, the security team requests three months of login records for a specific user to determine what actions they performed and when. This request relies on which component of the AAA framework?
A) Authentication
B) Authorization
C) Accounting
D) Federation

**Answer:** C
**Justification:** Recording and retrieving what actions a user performed is the accounting function of AAA, supporting forensic investigation.

**Q100.** A user successfully enters the correct username and password, but the system then checks whether that user is permitted to open the payroll application. This second check is an example of:
A) Authentication
B) Authorization
C) Accounting
D) Identification

**Answer:** B
**Justification:** Determining what an already-authenticated user is permitted to do is authorization, which occurs after authentication.

**Q101.** A login system locks an account for 30 minutes after five consecutive failed password attempts. This control is specifically designed to reduce the risk of:
A) Phishing
B) Brute-force/credential-guessing attacks
C) SQL injection
D) DNS spoofing

**Answer:** B
**Justification:** Lockout policies limit repeated login attempts, directly mitigating brute-force password-guessing attacks.

**Q102.** A cloud administrator requests temporary elevated permissions to troubleshoot a production issue; the access is automatically granted for two hours and then revoked, requiring a new request for any future need. This model is called:
A) Standing privileged access
B) Just-in-Time (JIT) access
C) Role-based access control only
D) Mandatory access control

**Answer:** B
**Justification:** Granting elevated access only for the limited time it's needed, then automatically revoking it, is Just-in-Time access.

**Q103.** A company's security policy prohibits IT staff from using their personal administrator accounts for daily email and web browsing, requiring a separate standard account for non-administrative tasks. This practice primarily supports:
A) Job rotation
B) Least privilege / reducing exposure of privileged credentials
C) Mandatory vacation
D) Risk transfer

**Answer:** B
**Justification:** Limiting the use of privileged accounts to only when truly necessary reduces the exposure and risk associated with those powerful credentials, supporting least privilege.

**Q104.** A retail company's point-of-sale application allows managers to override certain transactions, but the system requires the manager to physically insert their own badge and enter a separate PIN, distinct from the cashier's login. This layered requirement demonstrates:
A) Role-based access control combined with a secondary authentication step
B) Federated identity
C) Mandatory access control
D) Discretionary access control

**Answer:** A
**Justification:** Different permissions based on role (manager vs. cashier), enforced with an additional authentication step for sensitive actions, combines RBAC with layered authentication.

**Q105.** A government agency's classified network prevents users from copying files from a "Secret" labeled system to an "Unclassified" system, even if the user has clearance for both, because the system enforces information flow rules centrally. This enforcement is characteristic of:
A) Discretionary Access Control
B) Mandatory Access Control
C) Role-Based Access Control
D) Attribute-Based Access Control

**Answer:** B
**Justification:** Centrally enforced rules governing information flow between classification levels, which users cannot override, is a hallmark of MAC.

**Q106.** A company discovers during an audit that a former contractor's VPN account, which should have been disabled six months ago, was used to access the network last week. What process failure does this indicate?
A) Failure of provisioning
B) Failure of deprovisioning
C) Failure of authentication
D) Failure of federation

**Answer:** B
**Justification:** The account should have been disabled (deprovisioned) when the contract ended; its continued activity indicates a deprovisioning failure.

**Q107.** An organization's badge system logs every entry and exit from the server room, including the date, time, and individual's identity, creating a record reviewed monthly by security. This process primarily supports:
A) Authentication only
B) Physical accounting/audit trail
C) Risk transfer
D) Role-based access control

**Answer:** B
**Justification:** Logging physical access events for later review creates an audit trail, supporting accountability (the "accounting" concept applied physically).

**Q108.** A new employee's manager requests access to the finance reporting system on their behalf, but a separate finance director must approve the request before the account is actually created. This workflow illustrates:
A) Discretionary access control
B) An approval-based provisioning workflow supporting least privilege
C) Mandatory vacation
D) Federated identity

**Answer:** B
**Justification:** Requiring a distinct approver before granting access ensures appropriate oversight in the provisioning process, aligned with least privilege principles.

**Q109.** A biometric fingerprint scanner used for building entry occasionally fails to recognize an authorized employee's finger due to a minor cut, requiring them to use a backup PIN instead. This scenario illustrates a limitation known as:
A) A false acceptance
B) A false rejection (false negative)
C) A replay attack
D) A federation failure

**Answer:** B
**Justification:** When a legitimate, authorized user is incorrectly denied access by a biometric system, this is a false rejection (false negative).

**Q110.** A biometric system mistakenly grants building access to an unauthorized individual whose fingerprint pattern was similar enough to an authorized employee's. This is an example of:
A) A false rejection
B) A false acceptance (false positive)
C) A replay attack
D) Tailgating

**Answer:** B
**Justification:** Incorrectly granting access to an unauthorized individual is a false acceptance, a critical security failure in biometric systems.

**Q111.** A company's access control policy states that all requests for access to the customer database must be logged, reviewed by a manager, and re-certified every six months, in addition to requiring MFA for login. Which combination of concepts does this best represent?
A) Only authentication
B) Layered access governance combining provisioning, accounting, and recertification
C) Only physical security
D) Only risk transfer

**Answer:** B
**Justification:** The policy combines controlled provisioning, ongoing logging (accounting), and periodic recertification — a layered access governance approach.

**Q112.** A university grants library database access to any user whose IP address originates from within the campus network, regardless of who they are individually. This is an example of:
A) Role-based access control
B) Rule-based access control
C) Mandatory access control
D) Discretionary access control

**Answer:** B
**Justification:** Granting access based on a defined condition/rule (originating IP range) rather than individual identity or role is rule-based access control.

**Q113.** During a security review, it's discovered that dozens of employees who changed departments over the past two years still retain access rights from their previous roles, resulting in excessive accumulated permissions. This situation is best described as a failure to:
A) Enforce mandatory access control
B) Conduct periodic access recertification and update permissions upon role change
C) Implement biometric authentication
D) Enforce dual control

**Answer:** B
**Justification:** Regular access reviews (recertification) would have identified and removed outdated permissions as employees changed roles — this is "privilege creep" resulting from a lack of recertification.

**Q114.** A company deploys a solution that requires administrators to check out a one-time-use password for a privileged account from a secure vault, which automatically changes the password after each use. This directly supports:
A) Role-based access control
B) Privileged Access Management
C) Federated identity
D) Rule-based access control

**Answer:** B
**Justification:** Managing, rotating, and controlling checkout of privileged account credentials is the core function of PAM.

**Q115.** A visitor at a secure facility uses a stolen access badge to enter through a turnstile that only reads the badge without verifying the person's identity against a photo. What additional control would have most likely prevented unauthorized entry?
A) A second authentication factor, such as a PIN or biometric check paired with the badge
B) A stronger Wi-Fi password
C) An intrusion detection system
D) A stronger backup policy

**Answer:** A
**Justification:** Pairing the badge (something you have) with a PIN or biometric (something you know/are) would have provided multi-factor verification, preventing entry with a stolen badge alone.

**Q116.** A cloud-based HR platform grants an employee access to their own payroll record but denies access to any other employee's record, and this rule applies identically to every employee in the company. This access enforcement is:
A) Discretionary access control
B) Rule-based access control (row-level restriction applied uniformly)
C) Mandatory access control
D) Physical access control

**Answer:** B
**Justification:** A uniformly applied rule ("users can only see their own record") enforced for all users is a form of rule-based access control.

---

## Domain 4: Network Security

**Q117.** A network engineer troubleshoots an issue where two devices on the same switch cannot communicate, despite having correct IP addresses, and discovers the physical cable is damaged. Which OSI layer does this issue relate to?
A) Layer 1 (Physical)
B) Layer 3 (Network)
C) Layer 4 (Transport)
D) Layer 7 (Application)

**Answer:** A
**Justification:** A damaged cable is a physical medium issue, corresponding to the Physical layer (Layer 1) of the OSI model.

**Q118.** A router receives a packet destined for a different subnet and forwards it based on the destination IP address in the packet header. This forwarding decision occurs at which OSI layer?
A) Layer 1
B) Layer 2
C) Layer 3
D) Layer 4

**Answer:** C
**Justification:** Routing decisions based on logical (IP) addressing occur at the Network layer (Layer 3).

**Q119.** A network switch receives an Ethernet frame and forwards it to the correct port based on the destination MAC address stored in its forwarding table. This occurs at which layer?
A) Layer 1
B) Layer 2
C) Layer 3
D) Layer 4

**Answer:** B
**Justification:** Frame forwarding based on MAC addresses is a Data Link layer (Layer 2) function.

**Q120.** During a network capture, an analyst notices that a file transfer is being retransmitted and reordered correctly despite packet loss, ensuring reliable delivery. Which OSI/TCP-IP layer and protocol are most responsible for this behavior?
A) Network layer / IP
B) Transport layer / TCP
C) Data Link layer / Ethernet
D) Application layer / HTTP

**Answer:** B
**Justification:** TCP, operating at the Transport layer, provides reliable, ordered delivery through retransmission and sequencing.

**Q121.** A company deploys a device at the network perimeter that examines incoming and outgoing traffic and blocks any connection attempts that don't match an approved rule set, such as denying all inbound traffic except HTTPS to the web server. This device is a:
A) Switch
B) Router
C) Firewall
D) Hub

**Answer:** C
**Justification:** A device enforcing traffic rules to permit or deny connections is a firewall.

**Q122.** A SOC receives an alert from a monitoring tool indicating a potential SQL injection attempt against a web server, but the tool takes no action to stop the traffic — it only logs and alerts. This tool is most likely a(n):
A) IPS
B) IDS
C) Next-gen firewall in blocking mode
D) VPN concentrator

**Answer:** B
**Justification:** A tool that detects and alerts on suspicious activity without blocking it is an Intrusion Detection System.

**Q123.** A company upgrades its security tool so that, in addition to alerting on the SQL injection attempt, it now automatically drops the malicious packets inline before they reach the web server. This upgraded capability makes it a(n):
A) IDS
B) IPS
C) Passive sensor
D) Honeypot

**Answer:** B
**Justification:** A tool that actively blocks malicious traffic inline, rather than just alerting, is an Intrusion Prevention System.

**Q124.** An employee working from a coffee shop connects to the corporate network through an encrypted tunnel so that their traffic cannot be intercepted by others on the same public Wi-Fi. This technology is a:
A) VLAN
B) VPN
C) DMZ
D) NAT

**Answer:** B
**Justification:** Creating a secure, encrypted tunnel over an untrusted network (public Wi-Fi) to reach corporate resources is the function of a VPN.

**Q125.** A company with employees spread across three floors of a building wants to logically separate the Finance department's traffic from the Marketing department's traffic on the same physical switches, without running new cabling. The best solution is:
A) NAT
B) VLANs
C) A cold site
D) A honeypot

**Answer:** B
**Justification:** VLANs allow logical segmentation of traffic into separate broadcast domains regardless of physical switch/cabling layout.

**Q126.** A company hosts its public-facing website on a server placed in a separate network segment, isolated with firewall rules from the internal corporate network, so that if the web server is compromised, attackers cannot directly reach internal systems. This segment is a:
A) VLAN only
B) DMZ
C) VPN
D) Honeypot

**Answer:** B
**Justification:** A network segment that hosts public-facing services while isolating them from the internal network is a DMZ.

**Q127.** A small office has 20 devices but only one public IP address from its ISP. All devices can access the internet simultaneously because the router translates their private internal addresses to the single public address. This technology is:
A) DHCP
B) NAT
C) DNS
D) VLAN tagging

**Answer:** B
**Justification:** Translating multiple private internal addresses to a shared public address is Network Address Translation.

**Q128.** A company's IT team is upgrading the office wireless network and wants to select the most secure available protocol, offering stronger protections against offline password-guessing attacks than previous standards. They should choose:
A) WEP
B) WPA
C) WPA2
D) WPA3

**Answer:** D
**Justification:** WPA3 is the current strongest Wi-Fi security standard, providing improved protections including against offline dictionary/brute-force attacks.

**Q129.** A security audit of a warehouse finds that its wireless scanners still connect using an outdated protocol known to be easily cracked using widely available tools within minutes. This protocol is most likely:
A) WPA3
B) WPA2-Enterprise
C) WEP
D) 802.1X

**Answer:** C
**Justification:** WEP is a legacy, cryptographically broken wireless protocol easily cracked with commonly available tools.

**Q130.** An employee at a coffee shop connects to what appears to be the shop's free Wi-Fi, but it is actually a malicious access point set up by an attacker using the same network name to intercept traffic. This attack is known as:
A) ARP spoofing
B) An evil twin attack
C) DNS spoofing
D) A DDoS attack

**Answer:** B
**Justification:** A rogue access point mimicking a legitimate one to intercept user traffic is an evil twin attack.

**Q131.** A user notices the browser padlock icon and "https://" prefix when logging into their bank's website, indicating their session is encrypted. This protection is provided by:
A) IPSec
B) TLS/SSL
C) SNMP
D) ARP

**Answer:** B
**Justification:** TLS/SSL encrypts HTTP traffic between browser and server, resulting in HTTPS and the padlock indicator.

**Q132.** A network administrator disables Telnet access to all network switches and routers, replacing it with a protocol that encrypts the administrative session and credentials. This replacement protocol is:
A) FTP
B) HTTP
C) SSH
D) SNMP v1

**Answer:** C
**Justification:** SSH provides encrypted remote administrative access, replacing the plaintext Telnet protocol.

**Q133.** When an employee types "www.company.com" into their browser, a service translates that name into the corresponding IP address so the browser can connect to the correct server. This service is:
A) DHCP
B) DNS
C) ARP
D) NAT

**Answer:** B
**Justification:** Translating human-readable domain names into IP addresses is the function of DNS.

**Q134.** Users report being redirected to a fake banking website that looks identical to the real one, even though they typed the correct URL. Investigation reveals the company's DNS resolver cache was tampered with to return a malicious IP address for the bank's domain. This attack is:
A) ARP spoofing
B) DNS spoofing/cache poisoning
C) A man-in-the-middle attack over TLS
D) A brute-force attack

**Answer:** B
**Justification:** Corrupting DNS resolver records to redirect legitimate domain lookups to malicious IPs is DNS spoofing/cache poisoning.

**Q135.** When a new laptop connects to the corporate network, it automatically receives an IP address, subnet mask, default gateway, and DNS server settings without any manual configuration. This is enabled by:
A) DNS
B) DHCP
C) ARP
D) SNMP

**Answer:** B
**Justification:** Automatic assignment of IP addressing and network configuration is provided by DHCP.

**Q136.** Employees report intermittent network issues, and investigation reveals an unauthorized device on the network is handing out incorrect gateway addresses to other devices, causing some traffic to be redirected through the attacker's laptop. This is an example of:
A) A legitimate DHCP server malfunction only
B) A rogue DHCP server attack
C) An ARP cache timeout
D) A DNS zone transfer

**Answer:** B
**Justification:** An unauthorized device distributing malicious network configuration (like a fake gateway) to intercept traffic is a rogue DHCP server attack.

**Q137.** A device needs to send data to another device on the same local network and must first determine which physical (MAC) address corresponds to the destination's known IP address. This lookup uses:
A) DNS
B) ARP
C) DHCP
D) SNMP

**Answer:** B
**Justification:** Resolving an IP address to its corresponding MAC address on a local network is the function of ARP.

**Q138.** A penetration tester sends forged ARP messages on a local network, associating their laptop's MAC address with the default gateway's IP address, causing other devices to unknowingly send their traffic through the tester's machine. This technique is:
A) DNS spoofing
B) ARP spoofing/poisoning
C) NAT traversal
D) A DDoS attack

**Answer:** B
**Justification:** Forging ARP messages to redirect traffic through an attacker's machine is ARP spoofing/poisoning, often used to enable a man-in-the-middle attack.

**Q139.** An attacker positions themselves between a user and a legitimate website, intercepting and potentially modifying communications, while both parties believe they are communicating directly with each other. This describes a:
A) Denial-of-service attack
B) Man-in-the-middle attack
C) SQL injection attack
D) Cross-site scripting attack

**Answer:** B
**Justification:** Secretly intercepting and possibly altering communication between two parties who believe they're speaking directly is a man-in-the-middle attack.

**Q140.** An e-commerce site becomes completely unreachable after receiving a massive flood of traffic originating from thousands of compromised IoT devices around the world simultaneously. This attack is a:
A) Man-in-the-middle attack
B) Distributed Denial-of-Service (DDoS) attack
C) SQL injection attack
D) ARP spoofing attack

**Answer:** B
**Justification:** A flood of traffic from many distributed, compromised devices (a botnet) overwhelming a target is a DDoS attack.

**Q141.** A hospital network separates its medical device network, guest Wi-Fi, and administrative systems into distinct zones with firewalls between them, so that a compromise of the guest network cannot directly reach patient monitoring devices. This design principle is:
A) Defense in depth via network segmentation
B) Risk transfer
C) Federated identity
D) Mandatory vacation

**Answer:** A
**Justification:** Dividing a network into isolated zones to contain potential compromises is network segmentation, a form of defense in depth.

**Q142.** A company replaces its traditional port/IP-based firewall with a device capable of identifying specific applications (e.g., distinguishing Facebook traffic from general HTTPS traffic) and includes built-in intrusion prevention. This upgraded device is a:
A) Proxy server
B) Next-generation firewall (NGFW)
C) Hub
D) Basic packet filter

**Answer:** B
**Justification:** Application awareness combined with integrated IPS capability beyond basic port/IP filtering describes a next-generation firewall.

**Q143.** A school implements a device that intercepts all student web requests, checks them against a content filtering policy, caches frequently visited pages, and forwards approved requests on the students' behalf. This device is a:
A) Router
B) Proxy server
C) Switch
D) VPN concentrator

**Answer:** B
**Justification:** Acting as an intermediary that filters, caches, and forwards requests on behalf of clients is the function of a proxy server.

**Q144.** Before allowing any laptop to join the corporate network, a system checks whether the device has current antivirus definitions, the latest OS patches, and an active firewall; devices that fail are quarantined to a remediation network. This capability is called:
A) Network Access Control (NAC)
B) DNS filtering
C) NAT
D) VPN split-tunneling

**Answer:** A
**Justification:** Verifying device compliance with security policy before granting network access is the function of Network Access Control.

**Q145.** A financial institution redesigns its network so that every access request — whether from inside or outside the building — must be authenticated and authorized individually, with no location automatically treated as trusted. This approach reflects:
A) Perimeter-based security
B) A zero trust architecture
C) Discretionary access control
D) A flat network design

**Answer:** B
**Justification:** Requiring continuous verification for every access request regardless of network location, with no implicit trust, is the zero trust model.

**Q146.** A network administrator configures a switch so that only three specific, pre-approved MAC addresses can connect to a particular port; any other device plugged into that port is automatically shut down. This feature is:
A) VLAN tagging
B) Port security
C) NAT
D) DNS filtering

**Answer:** B
**Justification:** Restricting which MAC addresses may connect to a specific switch port is port security.

**Q147.** A startup rents virtual servers from a cloud provider, installing and managing its own operating system, middleware, and applications, while the provider manages the physical hardware, storage, and networking underneath. This cloud service model is:
A) SaaS
B) PaaS
C) IaaS
D) FaaS

**Answer:** C
**Justification:** Customer control over the OS and applications, with the provider managing underlying physical infrastructure, is IaaS.

**Q148.** A company subscribes to an online email service accessible via a web browser, where the provider manages everything from the hardware up through the application itself, and the customer only manages user accounts and data. This is:
A) IaaS
B) PaaS
C) SaaS
D) On-premises deployment

**Answer:** C
**Justification:** A fully managed application delivered over the internet, with the provider handling all underlying layers, is SaaS.

**Q149.** A hospital keeps its patient records system on infrastructure it fully owns and controls within its own data center, not shared with any other organization, due to strict regulatory requirements. This cloud (or non-cloud) deployment model is:
A) Public cloud
B) Private cloud (or on-premises)
C) Community cloud
D) Multi-tenant public cloud

**Answer:** B
**Justification:** Dedicated infrastructure used by a single organization, not shared publicly, describes a private cloud/on-premises deployment.

**Q150.** A company runs its everyday web application on a public cloud provider but keeps its most sensitive financial database on a private cloud, with data occasionally moving between the two environments as needed. This deployment model is:
A) Public cloud only
B) Hybrid cloud
C) Community cloud
D) SaaS only

**Answer:** B
**Justification:** Combining private and public cloud resources with data movement between them describes a hybrid cloud.

**Q151.** After migrating to an IaaS provider, a company's security team clarifies with the provider that while the provider secures the physical data center and hypervisor, the company remains responsible for patching its own virtual machine operating systems and securing its data. This division of responsibility is defined by:
A) The Business Impact Analysis
B) The shared responsibility model
C) The Code of Ethics
D) The RTO/RPO framework

**Answer:** B
**Justification:** Cloud providers and customers dividing security responsibilities based on the service model is defined by the shared responsibility model.

**Q152.** A basic firewall at a small business only examines the source IP, destination IP, and port number of each packet to decide whether to allow or block it, without inspecting the actual content of the traffic. This is a:
A) Next-generation firewall
B) Packet-filtering firewall
C) Web application firewall
D) Proxy firewall

**Answer:** B
**Justification:** Filtering based solely on header information like IP addresses and ports, without deep content inspection, describes a basic packet-filtering firewall.

**Q153.** A company notices unusual traffic patterns and determines an attacker gained initial access to one workstation, then moved to other systems on the same flat network because there were no internal barriers preventing further movement. What design flaw contributed to this?
A) Overuse of encryption
B) Lack of network segmentation
C) Excessive use of MFA
D) Use of a hot site

**Answer:** B
**Justification:** A flat, unsegmented network allows attackers to move laterally without restriction once they gain an initial foothold; segmentation would have limited this movement.

**Q154.** A retailer's security team wants to ensure that even if an attacker breaches the perimeter firewall, they cannot easily reach the payment processing servers without passing additional independent security checks. Implementing internal firewalls and segmentation between network zones exemplifies:
A) Risk transfer
B) Defense in depth applied to network architecture
C) Federated identity
D) Mandatory vacation

**Answer:** B
**Justification:** Adding multiple, layered barriers within the network (not just at the perimeter) is defense in depth applied to network design.

**Q155.** A company's remote workers connect to internal file servers using an encrypted tunnel that routes only traffic destined for the corporate network through the tunnel, while general internet browsing goes directly out through the employee's home internet. This configuration is known as:
A) Full-tunnel VPN
B) Split-tunnel VPN
C) Site-to-site VPN
D) NAT traversal

**Answer:** B
**Justification:** Routing only specific (corporate) traffic through the VPN while other traffic goes directly to the internet is split-tunneling.

**Q156.** Two branch offices establish a permanent, encrypted connection between their respective firewalls so that devices on both networks can communicate securely as if on the same network, without individual users initiating VPN connections. This is a:
A) Remote-access VPN
B) Site-to-site VPN
C) Split-tunnel VPN
D) SSL VPN for individual users

**Answer:** B
**Justification:** A permanent encrypted connection between two networks (rather than individual user connections) is a site-to-site VPN.

**Q157.** A company's SOC observes a large volume of half-open TCP connections targeting a web server, consuming server resources and preventing legitimate connections. This is characteristic of a:
A) DNS spoofing attack
B) SYN flood (a type of DoS attack)
C) ARP poisoning attack
D) Evil twin attack

**Answer:** B
**Justification:** A flood of incomplete TCP handshakes (SYN packets without completing the connection) exhausting server resources is a SYN flood, a common DoS technique.

**Q158.** A network security appliance decrypts, inspects, and re-encrypts HTTPS traffic passing through it to detect hidden malware inside encrypted sessions before forwarding it to its destination. This capability is known as:
A) NAT
B) SSL/TLS inspection
C) DNS filtering
D) Port security

**Answer:** B
**Justification:** Decrypting and inspecting encrypted traffic for threats before re-encrypting and forwarding it is SSL/TLS inspection.

**Q159.** A company observes that its DNS servers are receiving an abnormally high volume of queries from thousands of different sources, all targeting a specific domain, appearing to be an attempt to overwhelm the DNS infrastructure itself. This is best described as a:
A) DDoS attack targeting DNS services
B) ARP spoofing attack
C) Evil twin attack
D) SQL injection attack

**Answer:** A
**Justification:** A flood of traffic from many sources aimed at overwhelming DNS infrastructure is a form of DDoS attack.

**Q160.** A security architect designing a new branch office network decides to place all wireless guest traffic on a separate VLAN with internet-only access and no route to internal servers. What security goal is primarily achieved?
A) Enabling federation
B) Limiting the attack surface and containing potential compromise of guest devices
C) Enabling mandatory access control
D) Eliminating the need for a firewall

**Answer:** B
**Justification:** Isolating untrusted guest traffic from internal resources reduces the risk that a compromised guest device could reach sensitive internal systems.

**Q161.** During an assessment, a security consultant identifies that internal DNS servers allow full zone transfers to any requesting IP address, potentially exposing the entire internal network map to an attacker. This misconfiguration is a:
A) Vulnerability that could aid network reconnaissance
B) A form of NAT
C) A required feature of DHCP
D) An example of proper segmentation

**Answer:** A
**Justification:** Unrestricted DNS zone transfers can reveal internal hostnames and IP addressing to attackers, aiding reconnaissance — this is a vulnerability, not a security feature.

**Q162.** A company's wireless network uses a single shared password for all employees, which has not been changed in over three years and is known by former employees. Which upgrade would most directly address this weakness while maintaining centralized control and accountability?
A) Switching to WEP for compatibility
B) Implementing WPA2/WPA3-Enterprise with individual, centrally managed credentials
C) Removing all wireless access entirely
D) Disabling encryption to simplify troubleshooting

**Answer:** B
**Justification:** Enterprise mode ties access to individual, centrally managed credentials (often via RADIUS), allowing revocation for specific users without changing a shared password for everyone.

**Q163.** A company deploys sensors throughout its network that passively analyze traffic for known attack signatures and anomalous patterns, generating alerts for the SOC team to investigate, without altering or blocking any traffic. This deployment is best described as:
A) An IPS deployed inline
B) An IDS deployed out-of-band/passively
C) A next-generation firewall
D) A VPN concentrator

**Answer:** B
**Justification:** Passive traffic monitoring for alerting without blocking is the defining trait of an out-of-band IDS deployment.

**Q164.** A company migrating to the cloud selects a provider offering pre-built development tools and a managed runtime environment, allowing developers to deploy custom applications without managing servers or operating systems. This service model is:
A) IaaS
B) PaaS
C) SaaS
D) On-premises

**Answer:** B
**Justification:** Providing a managed platform (runtime, tools) for deploying custom applications without managing underlying servers/OS is PaaS.

---

## Domain 5: Security Operations

**Q165.** A company labels its documents as "Public," "Internal Use Only," "Confidential," and "Restricted," applying stricter handling and encryption requirements as sensitivity increases. This practice is known as:
A) Risk transfer
B) Data classification
C) Vulnerability scanning
D) Change management

**Answer:** B
**Justification:** Categorizing data by sensitivity to apply proportional controls is data classification.

**Q166.** During a data classification review, a company determines that its unreleased merger and acquisition documents require the strictest handling, including encryption and need-to-know access, due to the severe impact of unauthorized disclosure. These documents would most likely be classified as:
A) Public
B) Internal Use Only
C) Confidential/Restricted
D) Unclassified

**Answer:** C
**Justification:** Highly sensitive information whose unauthorized disclosure would cause severe harm is typically classified at the highest level (Confidential/Restricted).

**Q167.** An organization encrypts all files stored on its file servers and databases using AES-256, ensuring that even if a hard drive is physically stolen, the data remains unreadable without the encryption key. This protects:
A) Data in transit
B) Data at rest
C) Data in use
D) Data in motion

**Answer:** B
**Justification:** Encrypting stored files on servers/databases protects data at rest.

**Q168.** A company enforces TLS encryption for all traffic between its web application and users' browsers to prevent attackers from intercepting login credentials as they travel across the internet. This protects:
A) Data at rest
B) Data in transit
C) Data in use
D) Data in storage

**Answer:** B
**Justification:** Protecting data actively moving across a network, such as via TLS, secures data in transit.

**Q169.** A financial application uses specialized secure enclave technology to keep sensitive calculations encrypted even while being actively processed in the server's memory, protecting against certain memory-scraping attacks. This protects:
A) Data at rest
B) Data in transit
C) Data in use
D) Data in the DMZ

**Answer:** C
**Justification:** Protecting data while it is actively being processed in memory is protecting data in use.

**Q170.** A company deploys a tool that monitors outbound email and USB transfers, automatically blocking any attempt to send files containing credit card numbers outside the organization without authorization. This tool is a:
A) SIEM
B) Data Loss Prevention (DLP) system
C) IDS
D) NAC solution

**Answer:** B
**Justification:** Monitoring and blocking unauthorized transmission of sensitive data is the specific function of DLP.

**Q171.** During an audit, a company discovers several unmanaged servers running outdated software that IT was previously unaware existed, having been set up by a department without informing IT. This gap highlights a failure in:
A) Data classification
B) Asset management/inventory
C) Business continuity planning
D) Federated identity

**Answer:** B
**Justification:** Not knowing that these assets existed reflects a failure to maintain a complete and accurate asset inventory, a core security operations function.

**Q172.** After implementing an automated asset discovery tool, a security team identifies 50 previously unknown IoT devices connected to the corporate network. Maintaining visibility into all such devices going forward primarily supports:
A) Risk transfer
B) Effective vulnerability management and patching, since unknown assets can't be secured
C) Data classification only
D) Mandatory vacation policies

**Answer:** B
**Justification:** Comprehensive asset visibility is a prerequisite for applying patches, monitoring, and other protective controls consistently across the environment.

**Q173.** Before deploying a change to a production database, a developer must submit a request describing the change, obtain approval from a change advisory board, and test it in a staging environment first. This process is:
A) Vulnerability management
B) Change management
C) Incident response
D) Data classification

**Answer:** B
**Justification:** Formally reviewing, testing, and approving changes before implementation is change management.

**Q174.** An organization discovers that an unapproved software update was pushed directly to production servers over the weekend, causing an outage, without any documented approval or testing. This incident reflects a breakdown in:
A) Data classification
B) Change management
C) Risk transfer
D) Federated identity

**Answer:** B
**Justification:** The lack of review, testing, and approval before the change was deployed represents a failure of the change management process.

**Q175.** A company documents the minimum required security settings — disabled guest accounts, enabled firewall, specific password policy — that every new Windows server must meet before being deployed into production. This documented standard is a:
A) Security baseline
B) Risk register
C) Business impact analysis
D) Access control list

**Answer:** A
**Justification:** A documented minimum set of required security configurations for systems is a security baseline.

**Q176.** After a critical vulnerability is publicly disclosed in a widely used software library, the security team identifies all affected systems, tests an available patch in a lab environment, and rolls it out to production within 72 hours per company policy. This entire process is:
A) Vulnerability scanning only
B) Patch management
C) Business continuity planning
D) Data classification

**Answer:** B
**Justification:** Identifying, testing, and deploying updates to remediate vulnerabilities is patch management.

**Q177.** A company rolls out a critical security patch directly to all production servers simultaneously without first testing it, and the patch causes a critical application to crash across the entire organization. What step in the patch management process was skipped?
A) Vulnerability scanning
B) Testing in a non-production environment before deployment
C) Data classification
D) Risk transfer

**Answer:** B
**Justification:** Testing patches in a controlled, non-production environment before wide deployment helps catch compatibility issues that could cause outages.

**Q178.** A SOC analyst reviews centralized logs showing failed login attempts, file access records, and firewall denials from across the organization to identify patterns indicating a coordinated attack. This activity is best supported by:
A) A SIEM system
B) A DLP system
C) A NAC solution
D) A VPN concentrator

**Answer:** A
**Justification:** Aggregating and correlating log data from multiple sources to detect security events is the core function of a SIEM.

**Q179.** After a SIEM correlates failed logins from multiple countries against the same account within a short time window, it automatically generates a high-priority alert for the SOC. This is an example of:
A) Vulnerability scanning
B) SIEM correlation and alerting on anomalous behavior
C) Change management
D) Data classification

**Answer:** B
**Justification:** Identifying anomalous patterns across correlated log data and generating alerts is exactly what SIEM correlation rules are designed to do.

**Q180.** A company runs an automated tool weekly that scans all servers and identifies missing patches, outdated software versions, and known weaknesses, producing a prioritized list for remediation. This activity is:
A) Penetration testing
B) Vulnerability scanning
C) Incident response
D) Business continuity testing

**Answer:** B
**Justification:** Automated identification of known weaknesses across systems, without actively exploiting them, is vulnerability scanning.

**Q181.** After the vulnerability scan identifies a potential weakness, the company hires an ethical hacker to actively attempt to exploit that weakness under controlled conditions to determine whether it could actually be leveraged by a real attacker. This activity is:
A) Vulnerability scanning
B) Penetration testing
C) Patch management
D) Asset management

**Answer:** B
**Justification:** Actively attempting to exploit identified weaknesses to validate real-world impact is penetration testing, distinct from passive vulnerability scanning.

**Q182.** A suspicious email attachment is automatically detonated in an isolated virtual environment to observe whether it attempts to contact external servers or modify system files, without risking the production network. This technique is:
A) Sandboxing/malware analysis
B) Patch management
C) Data classification
D) Access recertification

**Answer:** A
**Justification:** Safely executing suspicious code in an isolated environment to observe its behavior is sandboxing/malware analysis.

**Q183.** An organization's endpoint protection software automatically detects a known ransomware signature on a user's laptop, moves the infected file to a secure isolated location, and prevents it from executing. This capability is:
A) DLP
B) Antivirus/anti-malware quarantine
C) NAC
D) SIEM correlation

**Answer:** B
**Justification:** Detecting, isolating (quarantining), and preventing execution of known malicious files is the core function of antivirus/anti-malware software.

**Q184.** A company performs a full backup of all data every Sunday night, and each subsequent night captures only the data that changed since Sunday's full backup, meaning Wednesday's backup includes all changes from Monday through Wednesday. This backup strategy is:
A) Full backup only
B) Differential backup
C) Incremental backup
D) Continuous backup

**Answer:** B
**Justification:** Capturing all changes since the last full backup (growing larger each day) describes a differential backup.

**Q185.** A different company performs a full backup every Sunday, and each subsequent night captures only the data that changed since the previous night's backup, meaning restoring data on Thursday would require Sunday's full backup plus every incremental backup from Monday through Thursday. This strategy is:
A) Full backup only
B) Differential backup
C) Incremental backup
D) Snapshot backup

**Answer:** C
**Justification:** Capturing only changes since the most recent backup (whether full or incremental) is incremental backup, requiring the full chain to restore.

**Q186.** A company decides that despite taking longer and requiring more storage, it will perform a complete backup of all data every single night, because it wants to be able to restore from any single backup set without needing multiple prior backups. This is:
A) Incremental backup
B) Differential backup
C) Full backup
D) Continuous data protection only

**Answer:** C
**Justification:** Copying all data every time, simplifying restoration to a single backup set at the cost of time/storage, is a full backup strategy.

**Q187.** A disaster recovery consultant recommends that the company keep three total copies of critical data, store them on two different types of media, and ensure one copy is kept at a separate physical location from the primary site. This recommendation follows the:
A) CIA triad
B) 3-2-1 backup rule
C) RTO/RPO framework
D) AAA framework

**Answer:** B
**Justification:** Three copies, two media types, one offsite is the definition of the 3-2-1 backup rule, a best practice for backup resilience.

**Q188.** After implementing a new backup system, a company schedules quarterly drills in which IT staff attempt to fully restore critical systems from backup to verify the process works and data is recoverable. This practice addresses the risk that:
A) Backups might not actually be restorable when needed
B) Employees might forget their passwords
C) The firewall rules might be misconfigured
D) The DNS server might fail

**Answer:** A
**Justification:** Untested backups may be corrupted or incomplete; regular restoration drills confirm that backups can genuinely be relied upon during a real incident.

**Q189.** After several employees fall victim to a phishing campaign impersonating the IT helpdesk, the security team rolls out mandatory training modules and simulated phishing tests to help staff recognize similar attacks in the future. This initiative is:
A) Vulnerability scanning
B) Security awareness training
C) Change management
D) Data loss prevention

**Answer:** B
**Justification:** Educating employees to recognize and respond appropriately to threats like phishing is the goal of security awareness training.

**Q190.** An employee receives an urgent phone call from someone claiming to be the CEO, demanding an immediate wire transfer and pressuring the employee not to verify the request through normal channels due to "time sensitivity." This is a classic example of:
A) A brute-force attack
B) A social engineering attack (pretexting/business email compromise style)
C) A DDoS attack
D) ARP spoofing

**Answer:** B
**Justification:** Manipulating a person through impersonation, urgency, and authority to bypass normal verification procedures is social engineering.

**Q191.** After a security awareness campaign, phishing simulation click rates drop from 25% to 5% over six months, and employees increasingly report suspicious emails to IT security. This trend demonstrates:
A) A failure of technical controls
B) The effectiveness of administrative controls (training) in reducing human-related risk
C) A need for stronger encryption
D) A need for network segmentation

**Answer:** B
**Justification:** Improved employee behavior following training demonstrates that administrative controls (security awareness training) are effectively reducing human-related risk.

**Q192.** An internal audit team, independent from the IT department, reviews access logs, configuration settings, and policy compliance across the organization and issues a report identifying gaps that need remediation. This activity is:
A) Vulnerability scanning
B) Penetration testing
C) A security audit
D) Change management

**Answer:** C
**Justification:** Independent review and verification that controls are functioning correctly, with findings on non-compliance, describes a security audit.

**Q193.** During a security audit, auditors discover that critical system logs are only retained for seven days before being automatically deleted, making it impossible to investigate incidents discovered later. What operational practice should be updated?
A) Data classification scheme
B) Log retention policy
C) VLAN configuration
D) Federation trust settings

**Answer:** B
**Justification:** Retaining logs for an insufficient period limits the ability to investigate incidents discovered after the retention window; the log retention policy should be extended appropriately.

**Q194.** A company's asset management system flags a critical database server as still running an operating system that reached end-of-life and no longer receives security patches from the vendor. What is the most appropriate immediate security operations response?
A) Ignore it since it's still functioning
B) Prioritize upgrading/replacing the unsupported OS or apply compensating controls until it can be replaced
C) Disable all logging on the server
D) Grant all users administrator access to simplify management

**Answer:** B
**Justification:** Unsupported operating systems no longer receive security patches, creating growing risk; prioritizing an upgrade or applying compensating controls (isolation, monitoring) addresses this until replacement is possible.

**Q195.** A SOC uses automated tooling to correlate threat intelligence feeds with internal network traffic, automatically blocking connections to IP addresses known to be associated with active malware command-and-control servers. This process supports:
A) Data classification
B) Proactive threat detection and prevention using threat intelligence
C) Business continuity planning
D) Federated identity management

**Answer:** B
**Justification:** Using external threat intelligence to proactively identify and block known malicious infrastructure is a core security operations practice.

**Q196.** A company's malware analysis team identifies that a piece of ransomware encrypts files and then deletes Windows shadow copies to prevent easy recovery, information that is then shared with the backup team to strengthen backup isolation. This cross-team collaboration exemplifies:
A) Risk transfer
B) Integration between malware analysis and operational resilience (backup) practices
C) Mandatory vacation
D) Federated identity

**Answer:** B
**Justification:** Insights from malware/threat analysis directly informing and strengthening backup and recovery practices demonstrates integrated security operations.

**Q197.** A security operations center implements a policy requiring that all critical alerts be acknowledged within 15 minutes and investigated within one hour, with escalation to a manager if these timeframes are missed. This is an example of:
A) A risk register
B) An operational Service Level Agreement (SLA) for incident handling
C) A business impact analysis
D) A data classification scheme

**Answer:** B
**Justification:** Defined response and resolution timeframes with escalation procedures constitute an operational SLA for the SOC's incident handling process.

**Q198.** After a vulnerability scan identifies over 200 findings across the environment, the security team prioritizes remediation based on which vulnerabilities are actively being exploited in the wild, affect internet-facing systems, and have the highest severity ratings. This approach reflects:
A) Random remediation
B) Risk-based vulnerability prioritization
C) Data classification
D) Business continuity planning

**Answer:** B
**Justification:** Prioritizing remediation based on exploitability, exposure, and severity rather than addressing findings randomly is risk-based vulnerability management.

**Q199.** A company's data retention policy states that customer records must be securely destroyed (not just deleted) three years after the account is closed, in compliance with applicable regulations. Which security operations practice ensures this happens correctly?
A) Vulnerability scanning
B) Secure data disposal/destruction procedures
C) Change management
D) Network segmentation

**Answer:** B
**Justification:** Ensuring data is irrecoverably destroyed in accordance with retention policy requires defined secure disposal/destruction procedures, not simple deletion.

**Q200.** A company discovers during an internal review that decommissioned hard drives were sent to a recycling vendor without being wiped or physically destroyed, potentially exposing sensitive data. What security operations control failed?
A) Access recertification
B) Media sanitization/secure disposal procedures
C) Change management
D) Federated identity

**Answer:** B
**Justification:** Properly wiping or destroying storage media before disposal is media sanitization; failing to do so before sending drives to a third party is a secure disposal control failure.

---

*This practice exam is a study aid modeled on the ISC2 Certified in Cybersecurity (CC) exam outline and does not contain official ISC2 exam content. For official exam objectives, visit isc2.org.*
