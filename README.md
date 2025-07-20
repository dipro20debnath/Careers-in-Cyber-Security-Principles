# 🛡️ Zero Trust vs Trust but Verify

## Trust but Verify
- ✅ Meaning: 
  - কাউকে বিশ্বাস করা হচ্ছে, কিন্তু সেটাকে যাচাই (verify) করাও হচ্ছে।
- 🔍 Example:
  - Internal network থেকে database access allow, কিন্তু সব query logged.
  - IDS/IPS দিয়ে suspicious activity detect করা।
- 📌 Pros:
  - সহজে deploy করা যায়।
  - user experience ভালো থাকে।
- ⚠️ Cons:
  - insider threat বা misconfiguration overlook হতে পারে।
- 💡 Remember: 

---

## Zero Trust
- ✅ Meaning:
- কাউকেই ডিফল্টে বিশ্বাস করা হবে না। সব access verify করতে হবে।
- 🔍 Example:
- device internal network এ থাকলেও, user MFA করবে।
- microsegmentation: network কে ছোট ছোট অংশে ভাগ করে, প্রতিটি segment access check করবে।
- 📌 Pros:
- অনেক বেশি secure।
- insider attack, lateral movement কমায়।
- ⚠️ Cons:
- complex, implement করতে resources & planning দরকার।
- 💡 Remember:



---

## 🏰 Analogy
| Principle         | Castle example                           |
|-------------------|------------------------------------------|
| Trust but Verify  | castle ভেতরে যারা আছে, তাদের বিশ্বাস করা, মাঝে মাঝে চেক করা। |
| Zero Trust        | castle ভেতরে ঢুকতে হলেও বারবার পরিচয়, badge, password লাগবে। |

---

## 🔍 Key differences
| Trust but Verify              | Zero Trust                        |
|--------------------------------|-----------------------------------|
| কিছুটা বিশ্বাস করবে, পরে verify করবে | কাউকেই বিশ্বাস করবে না, সব verify করবে |
| example: internal network trusted | example: internal network device MFA |
| সহজ deploy                    | কঠিন, কিন্তু secure |

---

## 📝 Summary
- 🛠 **Trust but Verify:** 
- ভরসা করো, কিন্তু নজর রাখো।
- 🧱 **Zero Trust:** 
- ভরসা করো না, সবসময় প্রমাণ চাও।

---












# Careers in Cyber Security


## Main Roles
- 🛠 Penetration Tester (OSCP, eJPT)
- 🔍 SOC Analyst (SIEM, Splunk, ELK)
- 🏗 Security Engineer (firewall, risk)
- 📝 GRC (ISO27001, GDPR)
- 🔬 Malware Analyst (IDA, Ghidra)
- 🕵️ Digital Forensics (memory/disk)

## Common Skills
- Networking (TCP/IP, DNS)
- Linux & Windows
- Scripting (Python)
- Cyber frameworks (MITRE ATT&CK)

## Notes
- Pick a focus: red team vs blue team
- Build homelab / use TryHackMe
- Always document learning





# Defence-in-Depth


## Definition
Multiple layers of security controls to protect data & systems. If one layer fails, others still provide protection.

## Examples
- Firewall → IDS → AV → MFA → Encryption → Logging
- Like layers of an onion 🧅

## Why?
- No single control is foolproof.
- Slows down attackers & increases detection.

## Key layers
- Physical security
- Network controls
- Endpoint security
- Access controls
- Data encryption
- Monitoring & incident response
- Security policies & training
# Defence-in-Depth Analogy

## 🏰 Castle
- Moat -> outer wall -> guards -> inner wall -> keep -> treasury vault.
- Each layer slows or stops attackers.

## 🏦 Bank
- Security guard -> metal detector -> vault door -> individual lockers -> alarm system.

➡ If one layer fails, others still protect.









# ISO_IEC 19249_Design Principles

## 1. Least Privilege
- Just enough access. No extra.
- Example: Sales rep sees only prices.

## 2. Attack Surface Minimisation
- Turn off unneeded services.
- Example: Close unused ports.

## 3. Centralized Parameter Validation
- All input checks at one place.
- Example: Validate forms at gateway.

## 4. Centralized Security Services
- Auth, logs, crypto handled centrally.
- Example: Single Sign-On, SIEM.

## 5. Preparing for Error & Exception Handling
- Fail safe, don't leak info.
- Example: ATM fails safely on network error.







# Security Models

## Bell-LaPadula (Confidentiality)
- No Read Up (Simple Security)
- No Write Down (Star Security)
- WRITE UP, READ DOWN

## Biba (Integrity)
- No Read Down (Simple Integrity)
- No Write Up (Star Integrity)
- READ UP, WRITE DOWN

## Clark-Wilson (Integrity)
- CDI: data to protect
- UDI: external data
- TP: safe operations
- IVP: check validity






# Security Principles 

## CIA Triad
- 🔒 Confidentiality: encryption, access control
- 🛡 Integrity: hashing, digital signatures
- 🚀 Availability: backups, redundancy

## Defense in Depth
- Multiple layers: firewall → IDS → AV → endpoint hardening

## Least Privilege
- Users/services get minimal required permissions.

## Separation of Duties
- Split critical tasks across different people/roles.

## Audit & Accountability
- Enable logging, monitor logs, maintain evidence.

## Security through Obscurity
- Should NOT be main defense. Never rely solely on hiding info.

---

✅ **Room takeaway:**  
"Assume breach" mindset রাখো, always prepare with layered security & monitoring.

# DAD Triad (Disclosure, Alteration, Destruction)

## Disclosure
- Opposite of confidentiality
- Example: customer data leaked online

## Alteration
- Opposite of integrity
- Example: medical record changed

## Destruction / Denial
- Opposite of availability
- Example: ransomware, power cut shuts down network

---
✅ Goal: balance CIA to prevent DAD










# Vulnerability vs Threat vs Risk


## Vulnerability
- Weakness in system.
- Ex: Unpatched software, weak password.

## Threat
- Potential danger that can exploit vulnerability.
- Ex: Hacker, malware.

## Risk
- Likelihood + impact if threat exploits vulnerability.
- Ex: Data leak causes fines & loss of trust.

---

## Simple analogy
| Term         | Showroom case                  |
|--------------|--------------------------------|
| Vulnerability| Glass door                     |
| Threat       | Burglar who might break it     |
| Risk         | Chance of break-in + cost      |







