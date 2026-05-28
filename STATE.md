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
- **Docs sent:** POV Framework (May 2026), Customer References / anonymized findings deck (May 28), POV Framework Generic v4 (May 28)
- **Feedback from Archit:** Governance added as lead use case in POV — resolved
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
- **Deployment:** On-prem only — hard requirement, no SaaS
- **Pain:** Fully agent-based org with custom homegrown platform, zero governance layer
- **Use cases scoped:** Discovery · Governance · Activity logs · MCP gateway (privileged access)
- **Docs:** Scope & Use Case Doc (in progress)
- **Next step:** Sudeesh + engineer in-person visit to ZoomInfo India office. Non-prod environment first, then production.
- **Strategic note:** OEM potential. If they go commercial it sets a strong precedent.

### JB Poindexter
- **Type:** Design Partner
- **Stage:** Design Partner — active POC evaluation
- **Champion:** CISO
- **Deployment:** On-prem
- **Pain:** Agentforce, Copilot Studio, Claude Code agents with no governance
- **Competition:** iSoon.AI — ran POC first, wrapping up. We go second (advantage).
- **POC strategy:** Lead with Claude Code. Prescribe it, don't ask what tool they want. If Salesforce Chatter comes up, ask for exact requirements before committing — we have no Chatter integration built.
- **Contacts:** CISO (champion), John Barrow (internal driver), Luke (stakeholder)
- **Next step:** Discovery call on POC scope. Prescribe Claude Code. Engineering working on activity log for every user prompt.

### ZeroFox
- **Type:** Prospect (Haveli portfolio)
- **Stage:** Discovery
- **Champion:** Shon (CTO) — very engaged, has full ELT support
- **Technical owner:** Brian Ware (VP AI) — missed intro call due to scheduling conflict, back at work same day
- **Deployment:** Self-hosted / on-prem preferred
- **Pain:** Real Cursor-based security incident before Shon joined — agent scanned developer machines for plaintext passwords, caused a compromise. Deep AI transformation underway — eliminated entire middle management layer due to AI adoption. ~30 agents currently deployed. No governance layer.
- **Strategic angles:** (1) Bidirectional data sharing — ZeroFox does dark web credential intel, EOS does runtime enforcement. Strong precedent: Archit's prior CyberArk experience integrated with services like ZeroFox. (2) Third-party agent risk — ZeroFox does vendor risk, wants to extend to agents. EOS has a whole section on third-party agent risk. (3) MSSP/resell potential raised by Archit and Diego.
- **POC mode:** Self-hosted Docker container. Simple spin-up — ~5 minutes. Shon said to send info, he'll bring in his team to turn the wrench.
- **Contacts:** Shon (CTO · champion), Brian Ware (VP AI · technical owner)
- **Docs sent:** POV Framework Generic v4 (May 28) — sent alongside intro email to Brian
- **Next step:** Brian Ware discovery call early next week (Mon or Tue). Then full demo with Shon, Brian, IT, and product team.

### GoTo
- **Type:** Prospect (existing AppViewX CLM customer — warm intro via Vasu/Lucas)
- **Stage:** Discovery
- **Champion:** TBD — Dominic (Developer Experience) or Peter (Engineering Identity) likely
- **Deployment:** TBD
- **Pain:** AI adoption in all directions — top-down mandate and grassroots. Limited visibility today. GitHub Copilot governance exists in Thomas's org, rest ungoverned. They know the problem is real, don't know the scope.
- **Key context:** Not a security team — internal platform team. Lucas flagged post-call: "these guys aren't in security." Buying decision ownership unclear. Lucas going horizontal on the account.
- **Lucas:** Dinner with Dominique June 8 in Montreal — also pursuing S&P Global and Desjardins for same event. Diego should consider attending.
- **Next step:** Send recording + notes. Follow up after internal discussion. Loop through Lucas/Vasu weekly cadence with Thomas.

### Blend
- **Type:** Prospect (Haveli portfolio)
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
| POV Framework Generic v4 | General | External | Live — in GitHub repo |
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

**Lead story:** PocketOS — Cursor agent deleted a production database. ZeroFox had their own version (Cursor scanning for plaintext passwords). Real incidents, not hypothetical.

**Why we win:** Runtime enforcement (block, not just observe) · On-prem (trust signal) · 10-year machine identity foundation · Coding agents as the wedge · Governance as the category frame

**Governance vs PAM distinction:** Governance = IGA for agents (policy, ownership, posture, lifecycle). Privileged access control = PAM for agents (runtime enforcement at moment of execution). Same relationship, different layer. Archit has flagged governance as a top-level theme — it leads all positioning.

**Competitors:** iSoon.AI (in JBP POC — going second is an advantage), Oasis, Entro, CyberArk NHI, DIY

---

## Session Notes — May 28, 2026 (Evening)
- ZeroFox intro call processed — Shon (CTO) confirmed as champion, Brian Ware (VP AI) identified as technical owner
- ZeroFox had real Cursor-based incident (password scanning) — strong pain anchor
- ZeroFox POC agreed in principle — self-hosted Docker, Shon will bring in team
- Strategic angles confirmed: bidirectional data sharing, third-party agent risk, MSSP/resell
- POV Framework Generic v4 produced and pushed to GitHub repo
- POV updated throughout: governance as lead theme, "governed identity" in opener, EOS Guardian renamed to "the AppViewX agent sensor," SOC 2 removed, PAM/IGA distinction clarified in positioning
- Intro email sent to Brian Ware (cc Shon) — POV Framework Generic v4 attached
- ZeroFox docs sent tracker updated

---

## Session Notes — May 28, 2026 (GoTo addition)
- GoTo added as new deal (Discovery) — existing AppViewX CLM customer, warm intro via Vasu/Lucas
- Kashyap ran demo while sick, Suresh on PTO, Diego not yet leading — no discovery questions asked
- Platform team (not security) — Dominic and Peter likely internal owners
- Lucas going horizontal on account — dinner with Dominique June 8 Montreal, also pursuing S&P Global and Desjardins
- Key learning from this call: triggered Kashyap handing Diego the lead on all future external calls
