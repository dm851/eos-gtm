# Battle Card: Oasis Security

**Last updated:** May 28, 2026
**Category:** Pure-play NHI Governance Platform
**Stage:** Private — well-funded, strong analyst recognition
**Threat level:** HIGH — deepest pure-play NHI governance stack, directly competitive on discovery, lifecycle, and posture. New AAM product adds agentic access management. Weakest on machine identity (CLM/PKI) and on-prem deployment.

---

## What Oasis Claims

**Core NHI Platform:**
- Automatic discovery of all NHIs across cloud, SaaS, on-prem, and hybrid environments
- Contextual inventory enriched with ownership, usage, relationships, and blast radius
- Policy intelligence layer translating findings into business-relevant risk
- Full lifecycle governance: provisioning, rotation, migration, decommissioning
- Threat detection via Oasis Scout — behavioral anomaly detection for NHIs using AuthPrint fingerprinting
- Out-of-box remediation plans

**Agentic Access Management (AAM) — launched 2026:**
- Session-level governance for AI agent access — intent-aware, policy-driven
- Time-bound, JIT, and policy-driven access patterns for AI agents
- Sits between agents and the systems they touch across cloud, SaaS, and on-prem
- Ephemeral identity tracing from agent session creation to completion
- Audit trail per session with real-time activity logging

**Coverage:**
- IaaS: AWS, Azure, GCP, BigQuery
- SaaS: GitHub, ChatGPT, Salesforce, Office 365, Copilot
- On-prem environments

---

## What They Actually Do (Honest Assessment)

Oasis is the most mature pure-play NHI governance platform in the market. They have genuine depth on:
- NHI discovery breadth across hybrid environments
- Ownership attribution using AI and heuristics
- Lifecycle workflows that are actually implemented, not roadmap
- Secret rotation automation — customers have paused PAM projects after seeing Oasis
- Posture management and compliance reporting

AAM is a newer product launched in 2026, extending the NHI foundation to AI agents specifically. It's real and shipping, but earlier stage than the core NHI platform.

**Where Oasis is genuinely strong:** NHI posture management, secret rotation, lifecycle workflows, compliance coverage. Analyst recognition is well-earned.

---

## Where EOS Wins — The Genuine Gaps

### 1. No Machine Identity Foundation (CLM/PKI)
Oasis is a secrets and NHI governance platform. They do not manage certificates, PKI, SSH keys, or the cryptographic trust layer that underlies machine identity. AppViewX + EOS governs both the AI agent identity and the machine identity infrastructure it runs on — certificates, keys, and the full cryptographic trust chain. Oasis has half the picture.

**Reframe:** "Oasis governs what your agents can access. AppViewX also governs the cryptographic credentials your agents use to authenticate in the first place. One platform, full stack."

### 2. No MCP Gateway — Monitoring vs. Enforcement
Oasis describes their MCP approach as "direct-access rather than proxy-based" — they use native integrations to monitor and control agent activity through the identity layer. This is observability and policy enforcement at the identity level, not a gateway that intercepts and enforces at the protocol level. EOS's MCP gateway sits in the data path, intercepting every agent call before it reaches the target system.

**Reframe:** "Oasis monitors through the identity layer. EOS enforces at the protocol layer. When the agent makes a call it shouldn't, EOS blocks it. Oasis logs it."

### 3. On-Prem Deployment Depth
Oasis supports on-prem discovery through integrations, but their core platform architecture is cloud-native SaaS. For buyers who need agent telemetry to stay entirely on-prem — EOS was built for this from day one. Oasis's on-prem coverage is connection-based (they reach into on-prem environments from the cloud), not fully on-prem deployment.

### 4. No Coding Agent Endpoint Coverage
Oasis discovers agents through cloud APIs, SaaS integrations, and metadata analysis. Their discovery mechanism does not extend to live coding agent sessions on developer endpoints. The Claude Code / Cursor session-level governance problem is not in Oasis's coverage model.

**Reframe:** "Oasis discovers agents after they're deployed in cloud and SaaS. EOS governs what they do while they're running — including on developer endpoints."

### 5. Machine Identity + AI Agent on One Control Plane
Oasis is an NHI-only platform. Enterprises managing the 90-day TLS mandate, PQC migration, and AI agent governance simultaneously need to solve both problems. AppViewX + EOS is the only platform that addresses machine identity (certificates, PKI) and AI agent identity (governance, runtime enforcement) in a unified control plane. Oasis requires a separate CLM vendor alongside them.

---

## Common Objections and Responses

**"Oasis is the most mature NHI platform and has strong analyst coverage."**
Agreed — for NHI posture management and lifecycle governance of traditional NHIs (service accounts, API keys, OAuth tokens), Oasis has real depth. Where they stop is machine identity (certificates, PKI) and the AI agent runtime enforcement layer. EOS starts where Oasis's product ends.

**"Oasis has AAM for AI agents — doesn't that cover the use case?"**
AAM adds session-level governance for AI agents, which is real. The differentiation is in enforcement architecture: Oasis enforces through the identity layer (policy applied at the identity provider level), EOS enforces at the MCP protocol layer (gateway intercepts the call). Also: EOS has AppViewX's 10-year machine identity foundation underneath it. Oasis doesn't have an answer for certificate lifecycle or PKI.

**"Oasis discovered all our NHIs already — why bring in another tool?"**
Oasis's discovery is strong. The question is what you do after discovery. EOS's governance and enforcement layer can work alongside Oasis's discovery in some architectures — but for buyers looking for one platform across machine identity + NHI + AI agent governance, AppViewX + EOS is the only unified answer.

**"Oasis supports on-prem environments."**
Oasis connects to on-prem environments from their cloud platform — they reach in through APIs and integrations. EOS deploys the full platform on-prem. For CISOs who require zero telemetry to leave the environment, that distinction matters significantly.

---

## The Positioning Line

Oasis is the best pure-play NHI posture platform. EOS extends into AI agent runtime enforcement, MCP gateway control, and machine identity (certificates, PKI) — making it the only unified control plane for the full machine and agent identity problem. Oasis solves visibility and posture. EOS solves enforcement and trust.

---

## Account Intel — When Oasis Is Already Deployed

- Lead with machine identity gap — if they have a CLM problem alongside NHI, EOS + AppViewX is the unified answer
- MCP gateway vs. identity layer enforcement is the key technical differentiation to establish
- Coding agent endpoint coverage is not in Oasis's model — strong wedge for the developer security buyer
- Oasis customers who want to expand into CLM/PKI or PQC are natural AppViewX expansion targets

---

## Threat Assessment

**Where they win:** Pure NHI posture, secret rotation, compliance-driven buyers, cloud-native environments, accounts where CLM is handled separately.

**Where we win:** Machine identity + agent identity unified, MCP gateway enforcement, on-prem deployment, coding agent session governance, 90-day TLS + PQC + AI agent governance in one motion.

