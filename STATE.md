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
- **Docs needed:** Executive Readout Template
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
- **Next step:** Sudeesh + engineer in-person visit to ZoomInfo India office. Non-prod environment first, then production. Confirm OEM structure before visit.
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
*Structured as Project Earth GTM Readiness workstreams. Source of truth: Project Earth deck (May 2026).*

### MARKET READINESS

#### Website Updates & PR Release
- Owner: Alex (Marketing) — Diego coordinates
- Target: June 16, 2026
- Next: Confirm messaging alignment with Alex before publish. Ensure Diego is looped on all copy.

#### Analyst Briefings
- Owner: Alex (Marketing)
- Target: TBD — likely post-Identiverse
- Next: Get date from Alex. Prepare design partner proof points.

#### Sales Collateral
- Owner: Diego · Alex (Marketing)
- Includes: EOS one-pager, ICP one-pager, discovery card, demo journey, exec readout template, category positioning doc, POV framework
- Docs live: POV Framework Generic v4 (GitHub), Demo Journey HTML (GitHub)
- Next: EOS one-pager and ICP one-pager first — needed for June 10. Exec readout before Broadridge Week 4.

#### Lead Capture & Nurture
- Owner: Catherine Weaver · Alex (Marketing)
- Trigger: Automated routing activates when AIS landing pages go live (6/16)
- Routing: All AIS inbound leads go to Diego initially
- Next: Confirm routing setup with Catherine before 6/16.

---

### ENABLEMENT READINESS

#### Internal GTM Enablement
- Owner: Diego · Megan Davis
- Date: June 10, 2026
- Objectives: EOS story · 60-sec elevator pitch · Inbound handling · Opp routing · Roles clarity · 3 Whys
- Next: Finalize enablement deck. Distribute ICP one-pager and discovery card on the day.

#### Channel Announcement
- Owner: Diego · Troy Gankworth
- Goal: Identify 3–5 channel partners to enable on AIS. GuidePoint as anchor.
- Includes: Channel bounty program (incentivize individual reps to refer DP candidates)
- Next: Develop bounty concept with Troy. Tie announcement to 6/16 PR if possible.

---

### PIPELINE CREATION READINESS

#### Opportunity Sourcing
- Owner: Diego
- ICP hypothesis: High AI adoption · Large dev orgs · Multi-cloud · FinTech · AI-native · Security-conscious CISOs
- Current: 4 DPs · ZeroFox + GoTo in discovery · Blend, Couchbase, FedEx, Orbia as prospects
- Warm pipeline: Haveli portfolio (~10 companies)
- Next: Map Haveli portfolio against ICP. Finalize ICP definition. Evaluate BDR resource. Build DP outreach sequence.

#### GTM Roles & Responsibilities
- Owner: Diego · Catherine Weaver
- Status: Defined in Project Earth deck — prospecting and opportunity cycle documented
- Key rule: One voice per account. AIS GTM notifies AE before outreach. Catherine is escalation point.
- Next: Socialize with Devo and AE team before June 10. Include in enablement session.

#### AE SPIF Program
- Owner: Diego · Catherine Weaver
- Status: Defined in Project Earth deck — needs Catherine to operationalize in SFDC
- First 5 Customers: 1st $2K · 2nd $1.5K · 3rd $1K · 4th $750 · 5th $500
- Pipeline Champ: $1K for self-sourcing 5 deals · $200/deal beyond 5
- Next: Brief Catherine. Announce at June 10 enablement.

#### Lead Routing & SFDC Hygiene
- Owner: Diego · Catherine Weaver
- Tracking: Product Line field on Opportunity — tag all AIS opps
- Next: Confirm tagging convention with Catherine. Set up automated inbound routing before 6/16.

---

### PRICING & PACKAGING

#### Finalize Consulting Partner
- Owner: Archit · Paul
- Status: In progress
- Next: Get update from Archit on timeline. Be ready to provide DP input when asked.

#### Price Model & Packaging
- Owner: Archit · Paul · Diego
- Direction: Per-agent + credits model being considered. ASP hypothesis $75K. Tiers: Discover / Govern / Secure.
- Next: Participate in P&P meetings. Bring ZoomInfo, Broadridge, JBP deal context as anchors. Push for budgetary guideline before June 10.

---

### AI SALES OPS WORKFLOW

- Owner: Diego
- Scope: Call recording (Granola) · Auto recap pipeline (transcript → MEDDPICC update → Bible) · Auto-generated data sheets · SFDC hygiene automation
- Next: Define full workflow end-to-end before Monday. Identify toolchain: Granola → Claude → SFDC. Build recap pipeline first — highest immediate leverage.

---

## Documents Tracker

### External — Customer-Facing

**Broadridge**
- POV Framework — Sent May 2026
- Customer References / Anonymized Findings Deck — Sent May 28
- Executive Readout Template — NOT STARTED. Needed before Week 4 readout.

**ZoomInfo**
- Scope & Use Case Doc — In progress. Complete before India visit.

**Design Partner Agreements**
- Freshworks — Signed
- DocuSign — Signed
- JB Poindexter — Signed

**General / Multi-Account**
- POV Framework Generic v4 — Live in GitHub repo. Current version.
- EOS One-Pager — NOT STARTED. Needed by June 10.

---

### Internal — GTM Team

**Enablement (needed by June 10)**
- GTM Enablement Deck — Draft in progress. Owner: Diego + Megan Davis.
- ICP One-Pager for Reps — NOT STARTED. Needed for June 10 session.
- Discovery Card — NOT STARTED. Needed for June 10 session.

**Strategy and Operations**
- EOS GTM Bible (this document) — Live. Updated continuously.
- Haveli Portfolio ICP Map — NOT STARTED. Priority after Identiverse.
- Channel Bounty Program Brief — NOT STARTED. Owner: Diego + Troy Gankworth.

**Project Earth GTM Readiness Deck**
- Status: Internal planning document only. Framework and learning objectives captured in enablement/june-10-readiness.md in this repo.
- Five enablement slides still need to be built for June 10. See enablement/june-10-readiness.md for content brief.
- SPIF structure defined in deck — needs Catherine Weaver to operationalize in SFDC before June 10.
- Pipeline creation R&R defined in deck — needs to be socialized with Devo and AE team before June 10.

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

---

## Session Notes — May 28, 2026 (Project Earth restructure)
- Reviewed Project Earth GTM Readiness deck and transcript (internal call with Paul, Archit, Diego)
- Diego formally named as GTM coordinator for Project Earth — owns strategy and decisions across all workstreams
- Active Projects renamed and restructured to match Project Earth workstream naming exactly
- All previous custom project names absorbed into official AppViewX workstream buckets
- 13 projects across 5 buckets: Market Readiness, Enablement Readiness, Pipeline Creation, Pricing & Packaging, AI Sales Ops Workflow
- AI Sales Ops Workflow added as standalone Diego-led project — scope: call recording, auto recap, auto data sheets, SFDC automation — needed for Monday
- ZoomInfo OEM structure moved from Projects into ZoomInfo deal record
- Comp Plan removed from Projects (personal)
- index.html Projects section fully refactored to JS data-driven rendering — no more hardcoded HTML
- Chetna running broader incubation project from PM perspective — Diego plugging in
- Monday weekly and Project Earth cadence — Diego added to recurring meetings