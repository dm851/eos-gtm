# EOS GTM Bible — Current State
*Last updated: May 28, 2026*

Drop this file into any new chat alongside AGENT.md to restore full context instantly.

---

## GTM Status

| Milestone | Status |
|---|---|
| Soft launch · Identiverse | ✓ Done |
| Design partner validation | → Active (4 of 6–10 target) |
| First commercial · Broadridge POV | → Active |
| Sales enablement kickoff | → Jun 10, 2026 |
| Hard GA | Q4 2026 |

---

## Active Deals

### Broadridge
- **Type:** Commercial (first commercial deal)
- **Stage:** POV Active
- **Champion:** CISO (name TBC)
- **Deployment:** On-prem
- **Pain:** Unknown agents across 7 platforms, no runtime policy, no compliance coverage. Open gap: detecting Python scripts calling OpenAI APIs directly via terminal — in progress.
- **Platforms in scope:** GitHub Copilot, M365 Copilot, Security Copilot, Claude Code, OpenAI Codex, OpenAI on Bedrock, Agentforce
- **Docs sent:** POV Framework (May 2026), Customer References / anonymized findings deck (May 28)
- **Feedback from Archit:** Word "governance" missing from POV use cases — added
- **Next step:** 4-way sync (Diego, Kashyap, Suresh, Archit) to align on demo plan. Then schedule coding agent demo early next week.
- **MEDDPICC gaps:** Economic buyer not confirmed. Paper process not started.

### Freshworks
- **Type:** Design Partner
- **Stage:** Design Partner
- **Champion:** CTO
- **Deployment:** On-prem
- **Pain:** Claude Code / Cursor agents accessing prod systems without policy
- **Docs:** DP Agreement (signed)
- **Next step:** Claude Code / Cursor use case — active validation

### DocuSign
- **Type:** Design Partner
- **Stage:** Design Partner
- **Champion:** Head of Product Security
- **Deployment:** On-prem
- **Pain:** Cursor, GitHub Copilot, Crew AI accessing sensitive document workflows
- **Docs:** DP Agreement (signed)
- **Next step:** 4 use cases scoped — validation in progress

### ZoomInfo
- **Type:** Design Partner + potential OEM
- **Stage:** Design Partner
- **Champion:** Venkat (VP Apps & AI) · Ravi (direct report)
- **Economic Buyer:** Sudeesh (India office)
- **Deployment:** On-prem only — hard requirement
- **Pain:** Fully agent-based org with custom homegrown platform, zero governance layer
- **Use cases:** Discovery · Governance · Activity logs · MCP gateway
- **Docs:** Scope & Use Case Doc (in progress)
- **Next step:** Sudeesh + engineer in-person visit to ZoomInfo India office. Non-prod first.

### JB Poindexter
- **Type:** Design Partner
- **Stage:** Design Partner — active POC evaluation
- **Champion:** CISO
- **Deployment:** On-prem
- **Pain:** Agentforce, Copilot Studio, Claude Code agents with no governance
- **Competition:** iSoon.AI — ran POC first, wrapping up. We go second (advantage).
- **POC strategy:** Lead with Claude Code. Prescribe it, don't ask what tool they want. If Salesforce Chatter comes up, ask for exact requirements before committing — we have no Chatter integration built.
- **Contacts:** CISO (champion), John Barrow (internal driver), Luke (stakeholder)
- **Next step:** Tomorrow's call — discovery on POC scope. Prescribe Claude Code. Weekend: engineering working on activity log for every user prompt.

### ZeroFox
- **Type:** Prospect (Haveli portfolio)
- **Stage:** Discovery
- **Champion:** Sean (CTO) — very engaged, has full ELT support
- **Technical owner:** Brian Ware (VP AI) — was not on intro call
- **Deployment:** Self-hosted / on-prem likely
- **Pain:** Had a real Cursor-based security incident before Sean joined — agent scanned developer machines for plaintext passwords, caused a compromise. Deep AI transformation underway. ~30 agents currently deployed. No governance layer.
- **Strategic angles:** (1) Bidirectional data sharing — ZeroFox does dark web credential intel, EOS does runtime enforcement. (2) Third-party agent risk — ZeroFox does vendor risk, wants to extend to agents. (3) MSSP/resell potential raised by Archit.
- **Next step:** Diego emails Brian Ware recap + requests discovery call early next week. Then full demo with Sean, Brian, IT, and product team.

### Blend
- **Type:** Prospect (Haveli portfolio — 2nd level coordination)
- **Stage:** Prospect
- **Next step:** Second level coordination — discovery + demo

### Couchbase
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Outreach — discovery pending

### FedEx
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Early — qualify and map

### Orbia
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Early — qualify and map

---

## Active Projects

### Broadridge POV Execution
- Owner: Diego
- Status: Active
- Scope: 7 platforms · 30-day POV
- Next: 4-way sync first. Then schedule coding agent demo early next week.
- Docs: POV Framework (sent), Customer References (sent), Exec Readout Template (needed)

### ZoomInfo DP + OEM Track
- Owner: Diego
- Status: Strategic / Active
- Next: Sudeesh + engineer India visit. Non-prod first.
- Docs: Scope Doc in progress

### Sales Enablement Kickoff
- Owner: Diego + Megan Davis
- Date: June 10, 2026
- Next: Finalize enablement deck. ICP one-pager. Discovery card.
- Docs needed: ICP One-Pager, Discovery Card

### Design Partner Scale — 6–10 by October
- Owner: Diego
- Current: 4 active DPs + ZeroFox in discovery (Haveli)
- Warm pipeline: Haveli portfolio — Blend, SolidEye, Serenia, Syrian Labs also in pipeline
- Next: Map remaining Haveli portfolio against ICP. Evaluate BDR resource.

### Channel Partner Bounty Program
- Owner: Diego · Troy Gankworth
- Status: Planning — new
- Concept: Incentivize individual partner reps to refer design partner candidates before GA
- Next: Diego develops concept. Talk to Troy. Loop in Catherine if needed.
- Docs needed: Bounty Program Brief

### Comp Plan FY2026
- Owner: Diego · Catherine Weaver
- Status: Pending Diego review + formal doc
- Key numbers: 6 paying customers (50% weight), $10.8M pipeline / 144 opps (50% weight), ASP $75K, FY ends Jan 2027, 8-month proration from May
- Note: Draft says 7-month proration — correct to 8 months
- Next: Diego reviews, aligns with Kashyap, Catherine formalizes

---

## Documents Tracker

| Document | Account | Type | Status |
|---|---|---|---|
| POV Framework | Broadridge | External | Sent |
| Customer References (Anonymized) | Broadridge | External | Sent May 28 |
| Design Partner Agreement | Freshworks | External | Signed |
| Design Partner Agreement | DocuSign | External | Signed |
| Design Partner Agreement | JB Poindexter | External | Signed |
| Scope & Use Case Doc | ZoomInfo | External | In Progress |
| GTM Enablement Deck | Internal | Internal | Draft |
| EOS GTM Bible | Internal | Internal | Live |
| Executive Readout Template | Broadridge | External | Needed |
| EOS One-Pager | General | External | Needed |
| ICP One-Pager for Reps | Internal | Internal | Needed |
| Discovery Card | Internal | Internal | Needed |
| Haveli Portfolio ICP Map | Internal | Internal | Needed |
| Channel Bounty Program Brief | Internal | Internal | Needed |

---

## Key Positioning

**Lead story:** PocketOS — Cursor agent deleted a production database. ZeroFox had their own version of this (Cursor scanning for plaintext passwords). Real incidents, not hypothetical.

**Why we win:** Runtime enforcement (block, not just observe) · On-prem (trust signal) · 10-year machine identity foundation · Coding agents as the wedge

**Competitors:** iSoon.AI (in JBP POC — going second is an advantage), Oasis, Entro, CyberArk NHI, DIY

---

## Session Notes — May 28, 2026
- Processed 3 transcripts: Diego/Kashyap 1:1, ZeroFox intro, JBP/Broadridge internal prep
- ZeroFox moved from Prospect to Discovery — real incident, strong champion, Haveli forcing function
- JBP updated with POC strategy, iSoon.AI competitive intel, contact map
- Broadridge updated with second meeting notes, two docs now sent, governance gap flagged and fixed in POV
- Channel Bounty Program added as new project
- Comp plan documented as project
- Diego taking lead on all external calls going forward


Drop this file into any new chat alongside AGENT.md to restore full context instantly.

---

## GTM Status

| Milestone | Status |
|---|---|
| Soft launch · Identiverse | ✓ Done |
| Design partner validation | → Active (4 of 6–10 target) |
| First commercial · Broadridge POV | → Active |
| Sales enablement kickoff | → Jun 10, 2026 |
| Hard GA | Q4 2026 |

---

## Active Deals

### Broadridge
- **Type:** Commercial (first commercial deal)
- **Stage:** POV Active
- **Champion:** CISO (name TBC)
- **Deployment:** On-prem
- **Pain:** Unknown agents across 7 platforms, no runtime policy, no compliance coverage
- **Platforms in scope:** GitHub Copilot, M365 Copilot, Security Copilot, Claude Code, OpenAI Codex, OpenAI on Bedrock, Agentforce
- **Docs sent:** POV Framework (May 2026) — Drive link needed
- **Next step:** Agree POV start date. Name technical contact on Broadridge side. Confirm MDM access for Guardian plugin deployment.
- **MEDDPICC gaps:** Economic buyer not confirmed. Paper process not started. Decision process unknown.

### Freshworks
- **Type:** Design Partner
- **Stage:** Design Partner
- **Champion:** CTO
- **Deployment:** On-prem
- **Pain:** Claude Code / Cursor agents accessing prod systems without policy
- **Docs:** DP Agreement (signed)
- **Next step:** Claude Code / Cursor use case — active validation

### DocuSign
- **Type:** Design Partner
- **Stage:** Design Partner
- **Champion:** Head of Product Security
- **Deployment:** On-prem
- **Pain:** Cursor, GitHub Copilot, Crew AI accessing sensitive document workflows
- **Docs:** DP Agreement (signed)
- **Next step:** 4 use cases scoped — validation in progress

### ZoomInfo
- **Type:** Design Partner + potential OEM
- **Stage:** Design Partner
- **Champion:** Venkat (VP Apps & AI) · Ravi (direct report)
- **Economic Buyer:** Sudeesh (India office)
- **Deployment:** On-prem only — hard requirement, no SaaS
- **Pain:** Fully agent-based org with custom homegrown platform, zero governance layer
- **Use cases scoped:** Discovery · Governance · Activity logs · MCP gateway (privileged access)
- **Docs:** Scope & Use Case Doc (in progress)
- **Next step:** Sudeesh + engineer in-person visit to ZoomInfo India office. Non-prod environment first, then production.
- **Strategic note:** OEM potential. If they go commercial it sets a strong precedent.

### JB Poindexter
- **Type:** Design Partner
- **Stage:** Design Partner
- **Champion:** CISO
- **Deployment:** On-prem
- **Pain:** Agentforce and Copilot Studio agents with no governance
- **Docs:** DP Agreement (signed)
- **Next step:** Agentforce / Copilot Studio use case — active

### Blend
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Discovery — qualify champion

### Couchbase
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Outreach — discovery pending

### FedEx
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Early — qualify and map

### Orbia
- **Type:** Prospect
- **Stage:** Prospect
- **Next step:** Early — qualify and map

---

## Active Projects

### Broadridge POV Execution
- Owner: Diego
- Status: Active
- Scope: 7 platforms · 30-day POV
- Next: Agree start date. Name tech contact. Confirm MDM access.
- Docs needed: Executive Readout Template

### ZoomInfo DP + OEM Track
- Owner: Diego
- Status: Strategic / Active
- Next: Sudeesh + engineer India visit. Non-prod first. Confirm OEM structure before visit.
- Docs: Scope Doc in progress

### Sales Enablement Kickoff
- Owner: Diego + Megan Davis
- Date: June 10, 2026
- Audience: Full AppViewX sales team
- Next: Finalize enablement deck. Build ICP one-pager. Build discovery card.
- Docs needed: ICP One-Pager, Discovery Card

### Design Partner Scale — 6–10 by October
- Owner: Diego
- Current: 4 active
- Target: 6–10 by October 2026
- Warm pipeline: Haveli portfolio (~10 companies)
- Next: Map Haveli portfolio against ICP. Identify top 3 targets. Evaluate BDR resource.
- Docs needed: Haveli ICP Map, DP Outreach Sequence

---

## Documents Tracker

| Document | Account | Type | Status |
|---|---|---|---|
| POV Framework | Broadridge | External | Sent — Drive link needed |
| Design Partner Agreement | Freshworks | External | Signed |
| Design Partner Agreement | DocuSign | External | Signed |
| Design Partner Agreement | JB Poindexter | External | Signed |
| Scope & Use Case Doc | ZoomInfo | External | In Progress |
| GTM Enablement Deck | Internal | Internal | Draft |
| EOS GTM Bible | Internal | Internal | Live |
| Executive Readout Template | — | External | Needed |
| EOS One-Pager | — | External | Needed |
| ICP One-Pager for Reps | — | Internal | Needed |
| Discovery Card | — | Internal | Needed |
| Haveli Portfolio ICP Map | — | Internal | Needed |

---

## Key Positioning

**Lead story:** PocketOS — Cursor agent deleted a production database. No policy. No audit trail. No ownership. Every org running coding agents is sitting on the same risk.

**Why we win:**
- Runtime enforcement (block, not just observe)
- On-prem (telemetry never leaves — trust signal vs SaaS-only competitors)
- 10-year machine identity foundation
- Coding agents as the wedge (fastest time to value)

**Competitors:** Oasis (discovery only), Entro (secrets hygiene), CyberArk NHI (no MCP gateway), Okta/SailPoint (human IAM bolting on NHI), DIY (18+ months of eng)

---

## How To Update This File

After every session where deals changed, run:
```
Update STATE.md to reflect: [what changed]
Then push both index.html and STATE.md to GitHub.
```

