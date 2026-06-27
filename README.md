# RBI-SEBI-REGULATORY-TRACKER
[RBI_SEBI_Tracker_README.md](https://github.com/user-attachments/files/29403513/RBI_SEBI_Tracker_README.md)
# 📋 RBI / SEBI Regulatory Change Tracker
### AI-Assisted Prompt Engineering Project — Indian Banking & Financial Regulation

> **Author:** Arsh Gulia | FRM Certified | B.A. (Hons.) Business Economics, University of Delhi  
> **Domain:** Regulatory Compliance · Credit Risk · Liquidity Risk · ESG Risk · Prompt Engineering

---

## Overview

This project demonstrates the application of **structured AI prompt engineering** to extract, analyse, and track key RBI and SEBI regulatory circulars (2022–2024). Each circular is processed using a reproducible 5-step prompt methodology and the outputs are organised across 12 analytical dimensions in a structured Excel tracker.

This is not a generic summary project. Every circular was processed with a deliberately engineered prompt — specifying the AI's role, context, extraction task, output format, and the regulatory framework to anchor against. The prompts are fully documented and replicable.

---

## Circulars Covered

| # | Circular | Regulator | Date | Category | Impact |
|---|----------|-----------|------|----------|--------|
| 1 | Master Circular – IRACP Norms 2024-25 | RBI | Apr 2024 | Credit Risk / NPA | High |
| 2 | Master Circular – IRACP Norms 2023-24 | RBI | Apr 2023 | Credit Risk / NPA | Medium |
| 3 | Master Circular – Bank Finance to NBFCs | RBI | Apr 2024 | NBFC / Concentration Risk | High |
| 4 | Draft Disclosure Framework – Climate-Related Financial Risks | RBI | Feb 2024 | ESG / Climate Risk | Medium |
| 5 | Basel III LCR / NSFR Update – Small Business Customers | RBI | Feb 2022 | Liquidity Risk | Medium |
| 6 | SEBI BRSR Core Amendment – ESG Disclosures | SEBI | Jul 2023 | ESG / Reputational Risk | Medium |

---

## Prompt Engineering Methodology

Every circular was analysed using the same 5-step prompt template:

```
Step 1 — Role:      "You are a senior credit risk analyst / compliance officer..."
Step 2 — Context:   Circular reference, issuing body, date, covered entities
Step 3 — Task:      Exact extraction targets (NPA timelines / provisioning rates / capital impact)
Step 4 — Format:    Constrained output (table / numbered bullets / section references)
Step 5 — Framework: Regulatory anchor (Basel II/III, TCFD, IFRS S2, SEBI BRSR)
```

**Example prompt used for the IRACP 2024-25 circular:**
```
"You are a bank compliance officer. Extract from this RBI Master Circular:
(1) NPA classification timelines,
(2) provisioning % by asset quality category,
(3) income recognition rules,
(4) capital implications.
Output as structured bullet points with section references.
Framework: Basel II Standardised Approach."
```

All 6 prompts are documented in the **Prompt Log** sheet of the Excel tracker.

---

## Project Structure

```
rbi-sebi-regulatory-tracker/
│
├── RBI_SEBI_Regulatory_Tracker.xlsx   ← Main deliverable (5 sheets)
│   ├── Dashboard                       Summary stats + navigation
│   ├── Circular Tracker                Full 12-dimension analysis of all 6 circulars
│   ├── Prompt Log                      Exact AI prompts used — replicable methodology
│   ├── Capital Impact Matrix           Which circular affects which ratio, and how
│   └── Compliance Calendar             All deadlines sorted chronologically + status
│
└── README.md
```

---

## What the Excel Tracker Contains

### Sheet 1 — Dashboard
Project overview, summary statistics (6 circulars, 2 High Impact, 4 Medium, categories breakdown), and sheet navigation guide.

### Sheet 2 — Circular Tracker *(Main Database)*
For each circular, 12 fields are populated:
- Circular reference number and title
- Regulator (RBI / SEBI) and date issued
- Entities affected
- Key changes (AI-extracted, numbered)
- Capital / liquidity impact (direction and mechanism explained)
- Compliance date
- Risk category
- Impact level (High / Medium / Low)
- Affected ratios (CAR, PCR, LCR, ESG Score etc.)
- Source URL
- Analyst notes

### Sheet 3 — Prompt Log
The exact prompt used for each circular, displayed in a code-style format. Anyone can copy these prompts and replicate the extraction on the same or newer circulars.

### Sheet 4 — Capital Impact Matrix
A heatmap-style matrix showing which circulars increase (↑), decrease (↓), or do not affect (—) each key regulatory ratio: CAR/CET1, PCR, Gross NPA%, Net NPA%, LCR, NSFR, Large Exposure, ESG Score, Credit Spread, Capital Cost.

### Sheet 5 — Compliance Calendar
All regulatory deadlines sorted chronologically from 2022 to 2027, with status tracking (Implemented / In Progress / Upcoming) and a description of what action is required by compliance date.

---

## Key Regulatory Insights

**NPA Provisioning (IRACP 2023-24 & 2024-25)**
Standard asset provisioning for commercial real estate was raised from 0.75% to 1.00% in FY2024 — directly reducing distributable profit for CRE-heavy lenders (HDFC, PNB Housing, LIC Housing Finance).

**NBFC Bank Finance Circular 2024**
New mandatory sub-limit for banks' exposure to NBFCs where gold loans ≥50% of assets — a direct response to IL&FS and DHFL contagion risk. Positive for systemic stability, constraining for volume growth.

**Climate Disclosure Framework 2024**
India's first formal TCFD-aligned climate risk framework. Currently disclosure-only, but transition risk assets (coal, fossil fuel portfolios) are flagged for potential future risk-weight increases under Basel IV revisions.

**LCR Update 2022**
Run-off rate for SME deposits reduced from 10% to 7.5% (relationship-based). Lower run-off → higher LCR numerator → banks holding SME deposits need less HQLA buffer → slightly positive for lending capacity.

---

## Skills Demonstrated

- `Prompt Engineering` — Structured 5-step AI extraction methodology, documented and replicable
- `Regulatory Analysis` — Deep reading of RBI Master Circulars and SEBI amendments
- `Credit Risk` — NPA norms, provisioning frameworks, Basel II Standardised Approach
- `Liquidity Risk` — LCR, NSFR, HQLA under Basel III liquidity framework
- `ESG / Climate Risk` — TCFD framework, BRSR, IFRS S2 alignment
- `Information Architecture` — Structuring unstructured regulatory text into searchable database
- `Financial Modelling` — Capital impact analysis (CAR, PCR, LCR direction and mechanism)

---

## How to Extend This Project

To add a new circular:
1. Go to rbi.org.in → Notifications or sebi.gov.in → Circulars
2. Download or paste the circular text
3. Use the prompt template from Sheet 3 (Prompt Log), adapting Step 3 for the new subject matter
4. Add a new row to Sheet 2 (Circular Tracker) with the extracted output
5. Update Sheet 4 (Capital Impact Matrix) and Sheet 5 (Compliance Calendar)

The methodology scales to any number of circulars across any jurisdiction.

---

## References

- [RBI Notifications](https://www.rbi.org.in/Scripts/NotificationUser.aspx)
- [SEBI Circulars](https://www.sebi.gov.in/legal/circulars.html)
- [GARP FRM Study Materials — Part II: Market Risk, Credit Risk, Liquidity Risk](https://www.garp.org/frm)
- [TCFD Recommendations](https://www.fsb-tcfd.org/)
- [IFRS S2 Climate Disclosures](https://www.ifrs.org/issued-standards/ifrs-sustainability-disclosure-standards/)

---


