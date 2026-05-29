# Portfolio Case Studies — Gaurav Nigota
## Microsoft 365 Engineer

---

## Case Study 1 — Exchange Online Migration Support

**Role:** Migration Engineer (Support)
**Tools:** Exchange Online, Microsoft 365 Admin Center, PowerShell

### The Situation
A client organization was in the middle of a mailbox migration to Exchange Online. End users were running into issues mid-migration — emails not syncing, mailboxes stuck in a queued state, and some users unable to access their accounts during the cutover window.

### What I Did
- Monitored migration batch status in real time using the Microsoft 365 Admin Center and PowerShell
- Identified irregularities — stuck migration jobs, failed batches, and mailboxes with sync errors
- Diagnosed root causes for each failure type and applied targeted fixes to unblock them
- Coordinated with end users to confirm access was restored before closing each issue
- Ensured the overall migration completed on schedule without data loss

### The Outcome
All flagged mailboxes were successfully migrated. End users experienced minimal disruption, and the migration completed within the planned window.

---

## Case Study 2 — M365 Multi-Tenant Management via GDAP (TD SYNNEX)

**Role:** Microsoft 365 Engineer
**Tools:** Microsoft 365 Admin Center, GDAP, Intune, Entra ID

### The Situation
As part of a managed services team at TD SYNNEX, I supported multiple client M365 tenants simultaneously. Each client had unique configurations, compliance requirements, and day-to-day operational needs — all managed through Granular Delegated Admin Privileges (GDAP).

### What I Did
- Managed multiple client tenants using GDAP access, operating at Global Admin level where required
- Handled day-to-day M365 administration — user lifecycle, licensing, group management, and troubleshooting
- Configured and maintained **Intune compliance policies** to enforce device security standards across client endpoints
- Built and deployed **configuration profiles** for Windows devices — controlling settings like BitLocker, Windows Update rings, and app deployments
- Ensured each tenant's environment stayed clean, documented, and aligned with Microsoft best practices

### The Outcome
Clients received consistent, reliable M365 management without needing in-house expertise. Device compliance rates improved across enrolled endpoints, and day-to-day tickets were resolved faster with standardized processes in place.

---

## Case Study 3 — Email Security Hardening (GSPANN)

**Role:** Microsoft 365 Engineer
**Tools:** Exchange Online, DNS Management, Microsoft Defender for Office 365

### The Situation
The organization was experiencing email delivery failures — legitimate emails were being rejected or landing in spam. There were no proper authentication records in place, leaving the domain exposed to spoofing and phishing risks.

### What I Did
- Audited the existing DNS records and identified missing or misconfigured **SPF, DKIM, and DMARC** entries
- Published a correctly scoped **SPF record** to define authorized sending sources
- Generated and published **DKIM keys** via Exchange Online and validated signing was working correctly
- Configured a **DMARC policy** starting in monitor mode (`p=none`) to gather reporting data, then tightened it progressively to `quarantine`
- Set up and managed **user mailboxes, shared mailboxes**, and **Distribution Lists with dynamic membership rules** based on Azure AD attributes — eliminating the need for manual group management

### The Outcome
Email delivery failures dropped significantly. The domain was properly authenticated, reducing spoofing risk and improving deliverability to external recipients. Dynamic distribution lists removed ongoing admin overhead for the team.

---

*These case studies are based on real work. Company and client details have been generalized where appropriate.*
