# Domain 2: Business Continuity, Disaster Recovery & Incident Response — Study Notes
*(~10% of the ISC2 CC exam)*

## 1. BCP vs. DRP — don't mix these up

| | **Business Continuity Plan (BCP)** | **Disaster Recovery Plan (DRP)** |
|---|---|---|
| Focus | Keeping the **business** running (people, processes, critical functions) | Restoring **IT systems/infrastructure** |
| Scope | Broad — org-wide operations | Narrow — technical recovery |
| Example action | Moving staff to an alternate office, communicating with customers | Rebuilding servers, restoring from backup |

> Think: **BCP = business survives. DRP = IT gets rebuilt.** DRP is actually a *subset* of the broader BCP effort.

## 2. Key Recovery Metrics (very commonly tested)

| Term | Definition | Answers the question... |
|---|---|---|
| **RTO** (Recovery Time Objective) | Max acceptable **time** a system can be down | "How fast must we be back up?" |
| **RPO** (Recovery Point Objective) | Max acceptable **data loss**, measured in time | "How much data can we afford to lose?" → drives backup frequency |
| **MTD** (Maximum Tolerable Downtime) | Absolute max downtime before the business suffers serious/unacceptable harm | "At what point does this become catastrophic?" |
| **MTTR** | Mean Time To Repair/Restore — average time to fix something | Operational metric, not a planning target |
| **MTBF** | Mean Time Between Failures — average time a system runs before failing | Reliability metric |

> Relationship: **RTO should always be ≤ MTD.** RPO is about data loss; RTO is about downtime — they are *not* the same thing.

## 3. Alternate Site Types (recovery speed vs. cost trade-off)

| Site Type | Readiness | Cost | Recovery Time |
|---|---|---|---|
| **Hot site** | Fully equipped, real-time/near real-time data replication | $$$$ (highest) | Minutes to hours |
| **Warm site** | Partial equipment, periodically updated data | $$ | Hours to a couple of days |
| **Cold site** | Basic infrastructure only (power, HVAC, connectivity) — no equipment/data | $ (lowest) | Days to weeks |
| **Reciprocal/mutual aid site** | Agreement with another org to share facilities in an emergency | Variable | Variable |

> Memory trick: **Hot = ready to go. Warm = needs some setup. Cold = needs everything.**

## 4. Business Impact Analysis (BIA)

- Identifies **critical business functions**, their **dependencies** (systems, vendors, people), and the **impact of disruption** over time.
- Produces the data used to set RTO/RPO/MTD and prioritize recovery order.
- Comes **before** you build the BCP/DRP — you can't plan recovery until you know what matters most and how fast it needs to come back.

## 5. Incident Response Lifecycle (NIST model — know the order!)

1. **Preparation** — before anything happens: policies, IR team, tools, training, tabletop exercises.
2. **Detection & Analysis** — identify that an event is happening, confirm it's a real incident, assess scope/severity.
3. **Containment** — stop the spread (isolate infected systems, disable compromised accounts) *without* yet removing the root cause.
4. **Eradication** — remove the actual threat (malware, backdoor) and close the vulnerability that allowed it in.
5. **Recovery** — restore systems to normal operation, monitor closely for recurrence.
6. **Lessons Learned / Post-Incident Activity** — review what happened, what worked, what to improve.

> Mnemonic: **P**lan, **D**etect, **C**ontain, **E**radicate, **R**ecover, **L**earn → "**Please Do Cool Exercises, Really Learn**"

**Common exam trap:** Containment vs. Eradication —
- **Containment** = stop the bleeding (isolate).
- **Eradication** = remove the cause (delete malware, patch).

## 6. Backup Strategy Concepts (also tied to Domain 5, but relevant to DR)

| Type | What's backed up | Restore complexity |
|---|---|---|
| **Full** | Everything, every time | Simplest restore (1 backup set) |
| **Incremental** | Only changes since the *last backup of any kind* | Fastest to create, slowest/most complex to restore (need full + every incremental) |
| **Differential** | Only changes since the *last full backup* | Faster restore than incremental (need full + latest differential only) |

- **3-2-1 rule**: 3 copies of data, on 2 different media types, with 1 copy offsite.
- Backups must be **tested via restoration drills** — an untested backup is not a reliable backup.

## 7. Communication During a Disruption

- BCPs typically include a **crisis communication plan**: who notifies employees, customers, regulators, and media, and in what order.
- Clear, accurate, timely communication reduces panic and reputational damage.

## Fast-Recall Summary
- BCP = keep the business running. DRP = rebuild the tech.
- RTO = time to recover. RPO = data you can afford to lose. MTD = the breaking point.
- Hot/Warm/Cold sites = readiness vs. cost trade-off.
- BIA happens first — it tells you what's critical and drives your RTO/RPO targets.
- IR lifecycle order: Preparation → Detection & Analysis → Containment → Eradication → Recovery → Lessons Learned.
- 3-2-1 backup rule + always test restores.
