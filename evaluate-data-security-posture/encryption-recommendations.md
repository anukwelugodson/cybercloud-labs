# Encryption Recommendations — Cedarville Family Health

**Project source:** IBM SkillsBuild Capstone — Task 2: Apply file and drive encryption  
**Prepared by:** Anukwelu Amamchukwu Godson  
**Date:**  16/09/2025  

---

## One-line summary
I chose simple, effective encryption practices the clinic can implement quickly to protect patient data, and I explained why each choice meets HIPAA expectations.

---

## Why use encryption? (simple)
**IBM form answer:** *To comply with HIPAA regulations.*  
**Plain explanation:** Encryption scrambles data so only authorized people with the right key can read it. If a laptop or backup drive is stolen and it is encrypted, the thief cannot read patient files.

---

## Recommended encryption settings (by area)

### 1) Office computers (endpoints)
- **What:** Full-disk encryption (BitLocker on Windows).  
- **Type:** AES-256.  
- **Why:** If the single clinic PC or a laptop is stolen, full-disk encryption prevents access to files.

### 2) Email communications
- **What:** TLS 1.2+ for transport; for very sensitive messages consider S/MIME or PGP.  
- **Why:** TLS protects messages while they travel to suppliers or remote staff. S/MIME/PGP provide end-to-end protection for particularly sensitive exchanges.

### 3) Data in transit (web/APIs)
- **What:** TLS 1.2 or 1.3 for websites and API connections; VPN for remote access.  
- **Why:** Prevents eavesdropping on network connections.

### 4) Backups
- **What:** Server-side encryption with a managed KMS (e.g., SSE-KMS), plus optional client-side encryption before upload.  
- **Why:** Ensures backups stored in the cloud or on external media are unreadable without keys.

### 5) Data exchange between providers
- **What:** Use TLS and, where possible, mutual TLS (mTLS) or secure file transfer protocols with encryption.  
- **Why:** Keeps PHI safe when sending records to labs or other clinics.

---

## Key management (simple steps)
- Use a managed Key Management Service (KMS) from the cloud provider if using cloud backups.  
- Restrict access to keys to a small number of administrators.  
- Require MFA for all admin accounts that can manage keys.  
- Rotate keys at least annually or per policy.

---

## Implementation checklist (copy/paste friendly)
1. Enable BitLocker (AES-256) on the clinic PC and any laptop used for patient records.  
2. Configure cloud backups to use SSE-KMS (server-side encryption with managed keys).  
3. Ensure all supplier and web traffic uses TLS 1.2/1.3.  
4. Avoid sending PHI over plain email; use secure email gateway or S/MIME for very sensitive info.  
5. Create a short encryption policy document and train staff on what encryption means and why it matters.

---

## IBM form question inside Task 2 — Why should Cedarville use encryption to protect patient records?
**Answer chosen:** *To comply with HIPAA regulations.*  
**Why (plain):** HIPAA requires reasonable technical safeguards to protect e-PHI. Encryption is a core technical safeguard that prevents unauthorized disclosure if a device or backup is lost or stolen.

---

## Short note for non-technical readers
- **Encryption** = turning readable files into scrambled files that only the clinic (with the key/password) can read.  
- It is an essential, low-cost safeguard for a small clinic that holds patient data.
