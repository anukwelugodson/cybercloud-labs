# Risk Assessment — Cedarville Family Health

**Project source:** IBM SkillsBuild Capstone — Step 1: Evaluate data security posture  
**Prepared by:** Anukwelu Amamchukwu Godson  
**Date:**  16/09/2025  

---

## Short plain summary
I read the clinic documents and used them to identify real risks to patient data (PHI). For each risk I wrote the likely consequence if the clinic does nothing, and a practical recommendation the clinic can implement quickly.

---

## How I approached the risk assessment (plain steps)
1. Read the office manager email (describes current setup: one internet-connected PC; daily export to portable hard drive kept in purse).  
2. Read the Information Sharing Policy and Security Meetings Policy.  
3. Read the HIPAA Security Rule summary (focus: confidentiality, integrity, availability).  
4. Listed the clinic’s sensitive data (PHI, billing records, staff PII).  
5. For each threat I wrote: *What could happen?* and *What should they do?*  
6. Prioritized risks by impact and how easy the fixes are.

---

## Risk table — what I found (simple, clear)
| # | Risk | Consequence if unaddressed | Practical recommendation |
|---|------|----------------------------|-------------------------|
| 1 | Phishing attacks targeting employee email | Patient data leaked → reputation + legal trouble | Email filter, phishing training, MFA, incident playbook |
| 2 | Unauthorized access by former employees | Data breach → fines, lawsuits | Revoke accounts on termination, do regular access reviews |
| 3 | Theft of the portable backup hard disk drive | Loss or exposure of PHI → regulatory penalties | Stop portable HDD workflow; use encrypted cloud backups or locked on-site encrypted NAS |
| 4 | Ransomware attacks | Clinic systems encrypted, service disruption | Install AV/EDR, maintain offline encrypted backups, patch systems |
| 5 | Inadequate password management | Account compromise | Enforce strong passwords, use password manager, enable MFA |
| 6 | Hacking via unsecured network connections | Data exfiltration and theft | Secure Wi-Fi, firewall, VPN for remote access, network segmentation |

---

## IBM / SkillsBuild questions (risk & compliance) — my answers and why
I put the exact answers below as short, clear statements a non-technical person can understand.

### Q: Why is the lack of encryption a data and privacy issue at Cedarville?
**Answer chosen:** *Intruders can easily read unencrypted data, increasing the risk of unauthorized access.*  
**Why:** If someone steals the portable drive or breaks into the computer, unencrypted files are easy to open. Encryption makes the files unreadable without the key.

### Q: Why is unrestricted access to electronic health records a data privacy concern?
**Answer chosen:** *Unrestricted access leads to unauthorized viewing or alteration of patient records, increasing the risk of privacy violations.*  
**Why:** Only people who need the data should see it. If too many people have access, mistakes or misuse can happen.

### Q: Choose three external risks the clinic faces:
**Answer chosen:**  
- Theft of the portable hard disk drive used for backups  
- Hacking through unsecured network connections  
- Ransomware attacks performed using malicious software  
**Why:** These threats typically come from outside attackers or criminals (theft, hacking, malware). They are not caused by clinic staff actions.

### Q: What is the consequence of phishing attacks if not addressed?
**Answer chosen:** *Leaked patient information causing reputational damage.*  
**Why:** Phishing often steals credentials or installs malware that can expose PHI. Losing patient trust and facing fines are major risks.

### Q: Consequence of unauthorized access by former employees?
**Answer chosen:** *Legal and financial consequences because of data breaches.*  
**Why:** Former staff with live accounts can leak or misuse data; that leads to fines and loss of reputation.

### Q: Should Cedarville tolerate phishing risk?
**Answer chosen:** *No — because the damage to reputation and patient trust is too significant.*  
**Why:** Phishing is common but largely preventable with training + technical controls. It is not acceptable for a clinic holding PHI.

---

## IBM form checkboxes — Compliance with HIPAA Security Rule (my selections & short reason)
> Use these exact selections when filling the SkillsBuild form.

- **Reasonable and appropriate safeguards:** **No**  
  *Reason:* Clinic uses unencrypted portable HDD and has only one internet-facing computer — technical safeguards are missing.

- **CIA of e-PHI (Confidentiality, Integrity, Availability):** **No**  
  *Reason:* Confidentiality and integrity are not guaranteed (unencrypted backups, no access controls, no backups strategy).

- **Threat protection:** **No**  
  *Reason:* No formal risk assessment, no detection (logs/EDR) described.

- **Protect against impermissible disclosures:** **Yes**  
  *Reason:* Clinic has written Information Sharing Policy that limits disclosure to authorized people.

- **Ensure workforce compliance:** **Yes**  
  *Reason:* Clinic has mandatory security meetings and training policies (attendance tracked).

---

## Notes for the assessor / recruiter
This risk assessment shows I can read policies and a real scenario, map them to HIPAA concerns, prioritize the risks and give clear actions a small clinic can implement quickly.
