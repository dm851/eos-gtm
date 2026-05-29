# Battle Card: Palo Alto Networks / Idira (formerly CyberArk)

**Last updated:** May 28, 2026
**Category:** Enterprise Security Platform — Network + Cloud + Identity + AI
**Ticker:** PANW
**Threat level:** VERY HIGH — largest enterprise security platform in the world, now with identity (CyberArk acquired Feb 2026), AI gateway (Portkey acquired Apr 2026), endpoint AI security (Koi acquired Apr 2026), and CLM (NGTS/Venafi)

---

## What Happened: The Acquisition Stack

Palo Alto is no longer just a network security company. Since early 2026 they have assembled:

| Acquisition | Closed | What It Added |
|---|---|---|
| CyberArk | Feb 2026 ($25B) | PAM, NHI governance, secrets, workload identity — rebranded as Idira |
| Koi | Apr 2026 | Agentic endpoint security for coding agents and AI endpoint apps |
| Portkey | Pending (announced Apr 30, 2026) | AI Gateway — MCP/A2A enforcement, token routing, agent traffic governance |

They also launched **NGTS (Next-Generation Trust Security)** at RSA 2026 — a CLM platform targeting the 90-day TLS mandate and PQC migration. This is a direct AppViewX CLM competitor.

The combined platform is organized into three pillars:
- **Strata** — network security (NGFW, SASE, ZTNA)
- **Cortex** — security operations (XDR, SOAR, SIEM)
- **Idira** — identity security (PAM + NHI + AI agent governance + CLM)

And overlaid with **Prisma AIRS 3.0** — their AI security platform covering discovery, red teaming, posture, and agent runtime.

---

## What They Claim

**Idira (GA May 12, 2026):**
- Zero standing privilege and JIT access for human, machine, and AI agent identities
- AI-driven discovery of all identities, entitlements, and access paths
- Automated identity lifecycle governance from creation to decommission
- 300+ out-of-box integrations, 200+ alliance partners (inherited from CyberArk)
- Agent Identity Security: each agent gets a governed identity with scoped permissions and full audit trail
- Integrates natively with Prisma AIRS for runtime agent privilege enforcement

**Prisma AIRS 3.0 (announced RSA 2026):**
- Agent Discovery across cloud, SaaS, endpoints
- Agent Artifact Security (pre-deployment scanning)
- Agent Red Teaming (automated adversarial testing)
- Agent Runtime Security — detects tool misuse, memory manipulation, adversarial instructions
- AI Agent Gateway (limited preview): centralized enforcement for all agent traffic via Portkey
- Agent Identity Security via Idira: scoped permissions, audit trail per agent

**NGTS:**
- Certificate lifecycle management targeting 90-day TLS mandate and PQC
- Direct competitor to AppViewX CLM

---

## What They Actually Do (Honest Assessment)

**Idira is real and strong — with important caveats:**
- The PAM and NHI governance foundation (CyberArk) is proven, enterprise-grade, and widely deployed
- Zero standing privilege and JIT access are genuinely implemented
- Lifecycle governance (ownership, onboarding, decommission) is functional
- However: Idira is a rebranded + extended CyberArk. Integration with Portkey (AI Gateway) is pending close. Koi (endpoint AI security) closed April 2026. Many capabilities are "roadmap" or "limited preview" — not fully integrated

**Prisma AIRS Agent Gateway is the most direct EOS competitor — but it's not GA:**
- The AI Agent Gateway is in limited preview as of May 2026
- Portkey acquisition pending close — full integration timeline unknown
- Agent Identity Security via Idira integration with Prisma AIRS is on the roadmap, not complete
- "Industry's first unified enforcement layer" claim is marketing for a product that isn't fully shipped

**NGTS is a real CLM threat:**
- Targets the same 90-day TLS mandate urgency as AppViewX
- Built on identity infrastructure from the CyberArk acquisition
- Will leverage PANW's massive install base for cross-sell

---

## Where EOS Wins — The Genuine Gaps

### 1. Three Companies Stitched Together Is Not One Platform
Idira (CyberArk) + Prisma AIRS (PANW native) + Portkey (pending) + Koi (just closed) is an integration project, not a shipping product. Customers buying "the full PANW AI agent security story" today are buying a roadmap. EOS ships now, deploys now, and governs now. Ask any PANW rep: when is the unified agent identity + gateway + runtime enforcement story GA? The honest answer is H2 2026 at the earliest.

**Reframe:** "PANW has announced everything we do. They haven't shipped it yet."

### 2. Complexity and Cost at Enterprise Scale
CyberArk was already expensive and complex before PANW acquired it. Adding Prisma AIRS, Portkey, and Koi on top creates a multi-module, multi-contract, multi-deployment challenge. EOS deploys in a single environment, on-prem, in days. PANW's full agent identity story requires Idira licenses + Prisma AIRS licenses + AI Gateway (Portkey) add-on. The TCO conversation alone is a differentiation point.

**Reframe:** "The full PANW agent identity stack is three acquisition integrations and multiple license SKUs. EOS is one platform, one deployment, one contract."

### 3. On-Prem Still a Gap
PANW is cloud-native across all three pillars. Idira (CyberArk) had on-prem deployment options historically, but the Idira rebrand and roadmap is SaaS-first. Portkey is SaaS. Prisma AIRS is SaaS. For security-conscious CISOs who require agent telemetry on-prem, the PANW stack has no clean answer. EOS was built on-prem first.

**Reframe:** "Every piece of the PANW AI agent story is SaaS. If your CISO requires agent telemetry to stay in-environment, that conversation ends quickly."

### 4. Machine Identity / CLM Is Now a Battlefield — EOS + AVX ONE Is the Counter
NGTS is a real CLM threat. PANW is going after AppViewX's CLM base. The counter: AppViewX has 10 years of CLM depth, CA-agnostic architecture, and existing enterprise relationships PANW is trying to displace. NGTS is new, unproven, and built on identity infrastructure that was designed for PAM — not certificate automation. The 90-day TLS mandate and PQC migration require purpose-built CLM depth that PANW doesn't have yet.

### 5. Coding Agent Gap Remains
Koi was acquired to fill the endpoint/coding agent gap. As of May 2026, Koi is newly closed and not integrated. The coding agent governance story at the developer endpoint session level — the core Broadridge use case — is still a gap in the PANW stack. EOS's agent sensor at the endpoint is shipping today.

---

## Common Objections and Responses

**"We're already a CyberArk customer and moving to Idira."**
Idira is CyberArk rebranded with an extended roadmap. Your existing investment carries forward, but the AI agent governance capabilities — gateway, runtime enforcement, coding agent endpoint security — are either limited preview or pending acquisition integration. EOS fills the gap now while PANW builds toward their roadmap. What's your urgency on governing coding agents in the next 90 days?

**"PANW has everything in one platform."**
They have announced everything in one platform. The AI Gateway (Portkey) isn't closed. Koi just closed in April. Idira went GA May 12. The integrations between these three acquisitions haven't been fully built. Ask your PANW rep for a demo of unified agent identity governance + gateway enforcement + endpoint coding agent security in a single workflow. That demo doesn't exist yet.

**"PANW beat everyone to market with Prisma AIRS."**
AIRS has had AI application security since version 1. Agent Gateway and Agent Identity Security in version 3.0 are in limited preview. The gap between "announced" and "GA and integrated" is where EOS operates today.

**"PANW can bundle this with our existing security spend."**
Bundling is the PANW sales motion. The counter: bundling means you get what fits the bundle, not what's right for the use case. Purpose-built agent identity governance will always outperform a module added to a network security platform's licensing structure.

---

## The Positioning Line

PANW is building toward what EOS does today. They have the resources, distribution, and acquisitions to get there — probably by late 2026. If your buyer has urgency now, EOS is the answer. If they're willing to wait 12-18 months for PANW's integrations to mature, that's the risk to qualify against.

---

## Account Intel — When PANW Is Already Deployed

- Idira (CyberArk) customers: lead with the roadmap gap — they need AI agent governance now, not when Portkey integration ships
- Prisma AIRS customers: lead with on-prem requirement or coding agent endpoint gap
- NGTS / CLM competitive displacement: AppViewX has 10 years of depth and CA-agnostic architecture that PANW is trying to replicate from scratch
- Watch for PANW using platformization discounts to bundle AI agent security into renewals — understand what's actually in the bundle before the customer signs

---

## Threat Assessment

**Where they win:** Existing CyberArk install base (massive), enterprises consolidating on PANW platform, customers willing to wait for roadmap, large regulated enterprises with broad PANW relationships.

**Where we win:** Urgency now, on-prem requirement, coding agent governance at the endpoint, purpose-built vs. acquisition integration, CLM depth (AppViewX), simpler deployment and lower TCO for EOS-specific use case.

**The existential risk:** If PANW ships a fully integrated, GA agent identity + gateway + CLM stack by Q4 2026 at competitive pricing, the "purpose-built vs. acquisition" argument weakens. Win accounts now while the integration gap is real.

