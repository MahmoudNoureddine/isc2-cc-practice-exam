# Domain 4: Network Security — Study Notes
*(~24% of the ISC2 CC exam)*

## 1. The OSI Model (7 layers — know them cold)

| Layer | Name | Deals with | Example devices/protocols |
|---|---|---|---|
| 7 | Application | End-user services | HTTP, FTP, DNS, SMTP |
| 6 | Presentation | Data formatting/encryption | SSL/TLS, JPEG |
| 5 | Session | Managing sessions/connections | NetBIOS, RPC |
| 4 | Transport | Reliable/unreliable end-to-end delivery | **TCP, UDP** |
| 3 | Network | Logical addressing & routing | **IP, routers** |
| 2 | Data Link | Physical addressing (MAC) | **Switches, Ethernet, ARP** |
| 1 | Physical | Raw bits, cables, signals | Cables, hubs, NICs |

> Mnemonic (top to bottom): **A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing
> Mnemonic (bottom to top): **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way

- **Routers = Layer 3** (IP-based decisions). **Switches = Layer 2** (MAC-based decisions).
- **TCP** = reliable, connection-oriented (handshake, retransmission). **UDP** = fast, connectionless, no guarantee of delivery.

## 2. Core Network Security Devices

| Device | Function |
|---|---|
| **Firewall** | Filters traffic per rule set (allow/deny by IP, port, protocol) |
| **IDS** (Intrusion Detection System) | **Detects** and alerts on suspicious traffic — passive, doesn't block |
| **IPS** (Intrusion Prevention System) | **Detects AND blocks** malicious traffic inline — active |
| **NGFW** (Next-Gen Firewall) | Firewall + application awareness + built-in IPS + deep packet inspection |
| **Proxy server** | Intermediary that filters/caches/forwards requests on behalf of clients |
| **VPN concentrator** | Manages encrypted VPN tunnels |

> IDS = alarm only. IPS = alarm **and** locks the door.

## 3. Network Segmentation & Architecture

- **VLAN** — logically separates devices into different broadcast domains, regardless of physical location/cabling.
- **DMZ (Demilitarized Zone)** — isolated segment hosting public-facing services (web servers) so a compromise there doesn't directly reach the internal network.
- **NAT (Network Address Translation)** — translates private internal IPs to a shared public IP; also hides internal addressing structure.
- **Segmentation in general** — limits lateral movement; if an attacker breaches one zone, they can't automatically reach others. Supports **defense in depth**.
- **Zero Trust** — "never trust, always verify" — every access request is authenticated/authorized regardless of network location; no implicit trust just because a device is "inside."

## 4. VPN Types

| Type | Use case |
|---|---|
| **Remote-access VPN** | Individual user connects securely to corporate network |
| **Site-to-site VPN** | Two networks (e.g., branch offices) permanently connected via encrypted tunnel |
| **Full-tunnel** | ALL traffic routed through the VPN |
| **Split-tunnel** | Only traffic destined for corporate resources goes through the VPN; rest goes direct to internet |

## 5. Wireless Security

| Protocol | Status |
|---|---|
| **WEP** | Broken/obsolete — easily cracked, never use |
| **WPA** | Improved over WEP, but outdated |
| **WPA2** | Solid, widely used (AES encryption) |
| **WPA3** | Current strongest standard — better protection against offline password attacks |

- **Evil twin** — rogue access point mimicking a legitimate one to intercept traffic.
- **Enterprise mode (WPA2/3-Enterprise)** — uses individual, centrally managed credentials (via RADIUS) instead of one shared password — allows per-user revocation.

## 6. Common Network-Layer Attacks

| Attack | What happens |
|---|---|
| **DoS / DDoS** | Flood of traffic (single source / distributed botnet) overwhelms a target, killing availability |
| **SYN flood** | Type of DoS — floods target with incomplete TCP handshakes, exhausting resources |
| **Man-in-the-Middle (MITM)** | Attacker secretly intercepts/alters communication between two parties |
| **ARP spoofing/poisoning** | Forged ARP messages redirect local traffic through the attacker's machine (enables MITM) |
| **DNS spoofing/cache poisoning** | Corrupts DNS records to redirect users to malicious sites |
| **Rogue DHCP server** | Unauthorized device hands out malicious network config (fake gateway/DNS) |

> Know the "resolves what to what" chain: **DNS** = name → IP. **ARP** = IP → MAC. **DHCP** = auto-assigns IP/gateway/DNS settings.

## 7. Encryption in Transit

- **TLS/SSL** → HTTPS (encrypts web traffic).
- **SSH** → secure encrypted remote admin access (replaces insecure **Telnet**).
- **SSL/TLS inspection** — a security appliance decrypts, inspects, and re-encrypts HTTPS traffic to catch hidden threats.

## 8. Cloud Concepts

**Service models (who manages what):**

| Model | Customer manages | Provider manages |
|---|---|---|
| **IaaS** | OS, middleware, apps, data | Physical hardware, virtualization, network |
| **PaaS** | Applications & data only | OS, runtime, middleware, infrastructure |
| **SaaS** | Just user accounts/data | Everything else (full application) |

**Deployment models:**
- **Public cloud** — shared, third-party owned/managed (AWS, Azure, GCP).
- **Private cloud** — dedicated to a single organization.
- **Hybrid cloud** — mix of private + public, data can move between them.
- **Community cloud** — shared by organizations with common requirements (e.g., government agencies).

- **Shared Responsibility Model** — defines the split between what the cloud provider secures vs. what the customer must secure (customer responsibility increases as you move IaaS → PaaS → SaaS... actually decreases! Customer has *most* responsibility in IaaS, *least* in SaaS).

## 9. Access & Compliance at the Network Layer

- **NAC (Network Access Control)** — checks device compliance (patch level, AV status) before allowing network access; non-compliant devices get quarantined.
- **Port security** — restricts which MAC addresses may connect to a specific switch port.

## Fast-Recall Summary
- OSI: Router=L3, Switch=L2. TCP=reliable, UDP=fast/unreliable.
- IDS=detect only. IPS=detect+block.
- VLAN=logical segmentation. DMZ=isolates public-facing servers. NAT=hides/shares public IP.
- WPA3 > WPA2 > WPA > WEP (never use WEP).
- DNS=name→IP. ARP=IP→MAC. DHCP=auto-config.
- MITM/ARP spoofing/DNS spoofing/rogue DHCP = all about hijacking or redirecting traffic.
- IaaS/PaaS/SaaS = decreasing customer responsibility, increasing provider responsibility.
- Zero Trust = never trust by default, always verify.
