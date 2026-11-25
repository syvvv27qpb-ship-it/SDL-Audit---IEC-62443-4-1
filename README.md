# SDL Audit of a Remote Access Solution – IEC 62443-4-1:2018

University team project in the course *Auditing of IT Systems*.
We audit the **Secure Development Lifecycle (SDL)** of **RASol GmbH** and its product **SRASol (Secure Remote Access Solution)**. The audit runs in the auditor role:

- **Audit criteria:** IEC 62443-4-1:2018, *Secure product development lifecycle requirements* (8 practices, 47 requirements)
- **Audit methodology:** DIN EN ISO 19011:2018, *Guidelines for auditing management systems*
- **Regulatory context:** Regulation (EU) 2024/2847 (Cyber Resilience Act), used for the DM/SUM practices only

> **Language note:** The project deliverables and the case-study documents are in **German**, as required by the course. This README is in **English** for better accessibility.

> **Disclaimer:** RASol GmbH, SRASol and every person named in the case study are **fictional**.

---

## Project status

| Package | Role | Task | Status |
|---|---|---|---|
| 1 | Auditor | 3-year audit programme, audit plans, audit team and auditee roles (Excel) | Completed |
| 2 | Auditor | Audit criteria catalogue with required objective evidence (Excel) | Completed |
| 3 | Auditee | Answer another team's audit questions based on the case study | Planned |
| 4 | Auditor | Rate the auditee's answers against the evidence; management summary (≤ 300 words) | Planned |

---

## Completed: Package 1 – Audit programme and audit plans

### Audit programme 2027–2029
The programme covers all 47 IEC 62443-4-1 requirements over three years:

| Audit | Scope | Window |
|---|---|---|
| AP-27-00 | Baseline review of documentation (all practices) | Jan–Feb 2027 |
| AP-27-01 | Practice 1 – Security Management (SM) | Apr 2027 |
| AP-27-02 | Practices 6–7 – Defect Management (DM), Security Update Management (SUM) | Sep 2027 |
| AP-28-01 | Practices 2–4 – Security Requirements (SR), Secure by Design (SD), Secure Implementation (SI) | Mar 2028 |
| AP-28-02 | Practice 5 – Security Verification & Validation Testing (SVV) | Jun 2028 |
| AP-29-01 | Practice 8 – Security Guidelines (SG); re-audit of selected SM requirements | Mar 2029 |
| AP-29-02 | Closing audit: verify all open nonconformities | Sep 2029 |
| AP-FU / PR | Follow-up audits (≤ 3 months after a report) and an annual programme review | As needed / yearly |

**Sequencing rationale**
1. **Foundation first:** SM sets the process, roles and development environment that every other practice depends on.
2. **Highest risk early:** DM/SUM are barely documented in the case study, and the product is internet-facing with CRA reporting obligations.
3. **Engineering chain as one unit:** SR → SD → SI → SVV are audited on the same release and traced through DOORS.
4. **Outputs last:** SG builds on SR, SD and SVV results, followed by re-audits and the closing audit.

The programme also defines the audit team and its competencies, risks and opportunities, and KPIs (e.g. requirement coverage, closure rate of nonconformities). Each element is referenced to the matching ISO 19011 clause (5.1–5.7).

### Audit plans (AP-27-01 and AP-28-01)
Our assigned scope is **19 requirements: SM-1–SM-13, SD-1–SD-4 and SI-1–SI-2**. SR-1–SR-5 belong to AP-28-01 but are audited by an external IEC 62443 auditor using a separate checklist.

| | AP-27-01 – Security Management | AP-28-01 – Secure by Design / Secure Implementation |
|---|---|---|
| Date | 12–15 Apr 2027 | 6–9 Mar 2028 |
| Location | Hamburg on site; Rio de Janeiro remote | Rio de Janeiro on site; Hamburg remote |
| Duration / team | 4 days / 4 people | 4 days / 4–5 people |
| Focus | Development, test and delivery environment; code signing; supplier control; release gate | Traceability requirement → threat → design → code; sample check of SM-11/SM-12 |

The plans include a day-by-day schedule, work assignments, auditee roles and contact persons, deadlines, sampling approach, audit risks, a rating scheme and the reporting procedure, structured according to ISO 19011 clauses 6.2–6.7.

---

## Planned work

- **Package 2:** Finish the Excel catalogue that pairs each assigned requirement with the objective, verifiable evidence needed to rate it as *fulfilled*, *partially fulfilled* or *not fulfilled*.
- **Package 3 (auditee role):** Answer the audit questions prepared by our assigned auditor team, based on the case study.
- **Package 4:** Rate the auditee's answers against the defined evidence and write a management summary that ranks the security gaps by risk to guide a 2-year improvement roadmap.

---

## Repository structure

```
├── Auditprogramm_Auditplans_DE  # Package 1: audit programme, audit plans,  (DE)
├── Auditkriterien_Nachweise_DE  # Package 2: criteria and evidence catalogue (DE)
└── README.md
```

## References

- **[N1]** DIN EN ISO 19011:2018-10 – Guidelines for auditing management systems
- **[N2]** IEC 62443-4-1:2018 – Security for industrial automation and control systems, Part 4-1: Secure product development lifecycle requirements
- **[N3]** IEC 62443-4-2:2019 – Technical security requirements for IACS components (referenced for SR-3/SR-4)
- **[L1]** Regulation (EU) 2024/2847 – Cyber Resilience Act
- Case-study documents of the fictional RASol GmbH (RASol-0001 to RASol-SP-0003), provided by the course

## Team

Auditteam 9 – Mouheb Jounaidi, Takoua Askri