# Core Security Concepts — SOC Foundations

## 1) CIA, AAA, PPT

### CIA Triad
| Property | Meaning | Example |
|---------|---------|---------|
| **Confidentiality** | Only authorized users can access data | Encrypting data / Access permissions |
| **Integrity** | Data must remain correct and unchanged | Hashing, Digital Signatures |
| **Availability** | Systems and data must be accessible when needed | Backups, Load Balancers, Redundancy |
-  In short: Who can read a file (confi.)? Who can write to the file (Integrity)? Is 
the file always available for this read and write (Availability).

### AAA Model
| Part | Meaning | Example |
|------|---------|---------|
| **Authentication** | Proving who you are | Password / Biometric login |
| **Authorization** | What you are allowed to do | Read-only user vs Admin |
| **Accounting** | Tracking user activity | Logs of login, file access, commands |

### PPT (People, Process, Technology)
Security is not only tools — it includes:
- **People** → awareness, training, insider risks.
- **Process** → policies, procedures, incident response playbooks.
- **Technology** → firewalls, SIEM, antivirus, EDR.

*Cybersecurity succeeds only when the three work together.*

---

## 2) Least Privilege Principle
Users, services, and applications should have **only the minimum level of access required** to perform their job — nothing more.

### Why?
- Reduces attack surface
- Limits damage if an account is compromised
- Prevents accidental misuse

**Example:**  
A helpdesk employee can reset passwords but cannot delete users or access financial records.

---

## 3) Authentication
Authentication = Confirming **identity**.

> "Are you really who you claim to be?"

Examples:
- Username + Password
- Face / Fingerprint
- Digital Certificates
- OAuth Login (Login with Google)

---

## 4) Authentication Factors
Ways a system verifies identity. Divided into categories:

| Factor Type | Description | Example |
|-------------|-------------|---------|
| **Something You Know** | Knowledge | Password / PIN |
| **Something You Have** | Physical item | Smart Card / Token / OTP app |
| **Something You Are** | Biological | Fingerprint / Face Recognition |
| **Somewhere You Are** | Location-based | GeoIP / Device location |
| **Something You Do** | Behavioral | Typing pattern / Swipe gesture |

**Multi-Factor Authentication (MFA)** = Using **2+ factors** together.

---

## 5) Authorization
Authorization = Deciding **what the authenticated user is allowed to do**.

> "Now that we know who you are — what can you access?"

Examples:
- Read vs Write vs Execute permissions
- Normal User vs Admin
- Network segmentation (VLAN access)

*Authentication happens **first**, authorization happens **after**.*

---

## 6) DAC and RBAC

### DAC — Discretionary Access Control
- Owner of the resource decides who gets access.
- More flexible but **less secure**.

**Example:** File permissions on Windows/Unix where the file owner sets access.

### RBAC — Role-Based Access Control
- Access is based on **roles**, not individuals.
- Users are assigned to roles → roles have permissions.
- Easier to manage in large organizations.

**Example:**
- Role: `DatabaseAdmin` → Permissions: Read/Write DB  
- User `Ali` is assigned to `DatabaseAdmin`

| Feature | DAC | RBAC |
|--------|-----|------|
| Control | Resource owner | Administrator defines roles |
| Flexibility | High | Medium |
| Security | Lower | Higher (recommended) |

---

## 7) Accounting
Accounting = Logging + Monitoring + Auditing.

It answers:
- **Who** did something?
- **When** did they do it?
- **What** did they access/modify?

Examples:
- Windows Event Logs
- Linux Syslog
- SIEM (Splunk, ELK, QRadar) aggregating audit logs

*Accounting is essential for Forensics and Incident Response.*

---

