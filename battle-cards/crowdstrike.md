# Battle Card: CrowdStrike

**Last updated:** May 28, 2026
**Category:** Endpoint / Cloud / Identity Security Platform
**Ticker:** CRWD
**Threat level:** HIGH — dominant endpoint platform, strong NHI narrative, SGNL acquisition adds continuous authorization, massive Falcon install base creates expansion risk

---

## What CrowdStrike Claims

**Falcon Next-Gen Identity Security:**
- NHI discovery across cloud, on-prem, AI-agent platforms, and SaaS (GigaOm 5/5 score)
- Risk-adaptive access controls across human and NHI identities
- Continuous dynamic authorization via SGNL acquisition (closed early 2026) — real-time grant/revoke based on Falcon risk signals
- JIT access beyond Active Directory — extends to AWS IAM, Okta, and cloud identity systems

**Charlotte AI AgentWorks (launched RSA 2026):**
- No-code platform to build, test, deploy, and orchestrate custom security agents
- Integrates with Anthropic Claude, NVIDIA Nemotron, OpenAI GPT, Amazon Bedrock
- Partners: Accenture, Deloitte, Salesforce, Telefónica Tech
- Charlotte Agentic SOAR for orchestration and governance of those agents

**Prompt AI Agent Security (GA RSA 2026):**
- Real-time discovery and governance control plane for AI agents
- Extends Autonomous Security Intelligence into the agentic layer
- Full MCP server visibility — discovers and monitors MCP servers across the environment
- Policy enforcement on agent behavior at runtime

**Falcon Data Security:**
- Discovery, classification, and policy enforcement for AI interactions
- AI governance at the data layer

**SGNL Acquisition (Jan 2026):**
- Continuous Identity — real-time authorization that grants and revokes access dynamically
- Extends dynamic privilege to NHI and AI agents beyond traditional identity providers

---

## What They Actually Do (Honest Assessment)

CrowdStrike's strength is the Falcon platform and endpoint telemetry. Their NHI and AI agent security story is built on top of that foundation — which is both a strength (rich cross-domain signal correlation) and a weakness (endpoint-centric lens applied to an identity governance problem).

**What's real:**
- Falcon Identity Security has genuine NHI discovery across cloud and SaaS
- SGNL integration adds continuous authorization — real capability, not vaporware
- Prompt AI Agent Security has MCP server visibility and policy enforcement at GA
- Charlotte AI and AgentWorks are real products, but they govern security agents inside the Falcon platform — not enterprise AI agents broadly

**What's marketing:**
- "Comprehensive NHI discovery across AI-agent platforms" — the depth varies significantly by platform. Discovery breadth is wide; governance depth is shallower than pure-play NHI vendors
- AgentWorks is primarily about building security automation agents, not governing enterprise AI agents (Claude Code, Cursor, Agentforce) that your business is deploying
- Lifecycle governance (ownership assignment, onboarding workflows, offboarding) is weaker than dedicated NHI platforms like Oasis or EOS

---

## Where EOS Wins — The Genuine Gaps

### 1. CrowdStrike Is an Endpoint Security Company Doing Identity
CrowdStrike's heritage is endpoint detection and response. Their NHI and agent identity story is built by correlation of endpoint + cloud + identity telemetry through the Falcon Security Cloud. That's a different architectural approach than a purpose-built identity governance platform. The result: strong on detection and behavioral anomaly (their core competency), weaker on governance workflows, lifecycle management, and policy definition.

**Reframe:** "CrowdStrike will tell you when an agent did something wrong. EOS defines what it's allowed to do."

### 2. AgentWorks Governs CrowdStrike's Agents — Not Yours
Charlotte AI AgentWorks is a platform for building security automation agents that run inside the Falcon platform. It is not a platform for governing the coding agents, Agentforce agents, or Copilot Studio agents your engineering and business teams are deploying. The naming and framing conflates two different problems. When a customer says "CrowdStrike has agent governance," clarify which agents.

**Reframe:** "AgentWorks helps CrowdStrike customers build security agents. EOS governs the AI agents your engineering team already deployed."

### 3. No MCP Gateway as an Enterprise Control Plane
CrowdStrike has MCP visibility (Prompt AI Agent Security monitors MCP servers). They do not have an MCP gateway that sits in front of MCP servers and enforces access policy before the agent call executes. The distinction is monitoring vs. prevention. EOS's MCP gateway intercepts agent calls and enforces JIT access policy before any tool call completes.

**Reframe:** "CrowdStrike sees what MCP servers are doing. EOS controls what they're allowed to do."

### 4. On-Prem Blind Spot
Falcon is a cloud-native SaaS platform. Their telemetry pipeline, data processing, and governance workflows all route through the Falcon Security Cloud. For buyers with hard on-prem requirements (Broadridge, ZoomInfo, financial services with strict data residency), CrowdStrike has no answer. EOS deploys fully on-prem.

### 5. Coding Agent Endpoint Gap
CrowdStrike detects threats on endpoints, including detecting malicious processes launched by coding agents. They announced detection of a Claude Code malicious process chain in March 2026 (LiteLLM supply chain attack). Detection of a malicious event is not the same as governing what Claude Code or Cursor is allowed to access during a normal, authorized development session. The standing-privilege problem at the session level is not solved by endpoint detection.

---

## Common Objections and Responses

**"CrowdStrike has NHI security — GigaOm gave them a perfect score."**
GigaOm recognized CrowdStrike's NHI discovery breadth and their cross-domain correlation, which is genuinely strong. The scoring criteria for that report emphasizes detection and response. EOS's differentiation is governance depth, lifecycle management, and prevention — not detection. Ask: "Does CrowdStrike define what your AI agents are allowed to access, or does it tell you when they've accessed something problematic?"

**"SGNL gives CrowdStrike continuous authorization."**
SGNL is a real and interesting capability — continuous dynamic authorization that grants and revokes access in real time. It's strong for human and cloud workload identities. For AI agent governance specifically — defining agent personas, scoping MCP access, managing the agent lifecycle from onboarding through decommission — SGNL/Falcon doesn't have the same depth as EOS's purpose-built governance layer.

**"We already have Falcon everywhere. Why add another product?"**
Fair consolidation argument. Counter: Falcon is the best endpoint security platform in the world. It was not built to govern the identity and access behavior of AI agents. The coding agent use case — a developer running Claude Code with access to production systems — is an identity governance problem, not an endpoint security problem. You need both. They don't overlap.

**"CrowdStrike detected that Claude Code process chain attack."**
They did — and that's impressive endpoint security. But that was a supply chain attack where malicious code was injected. The Broadridge problem is different: Claude Code is legitimate, authorized, and doing exactly what it was configured to do — with too much access. Endpoint detection doesn't help when the agent is working as intended.

---

## The Positioning Line

CrowdStrike is the world's best endpoint + identity detection platform. EOS is an agent identity governance platform. Detection and governance are not substitutes. CrowdStrike tells you when something went wrong. EOS defines what's allowed in the first place.

---

## Account Intel — When CrowdStrike Is Already Deployed

- Falcon Identity Security customers: strong on detection, weaker on governance workflows — lead with lifecycle management and MCP gateway enforcement
- Lean on the on-prem requirement if present — instant disqualifier for Falcon
- Clarify AgentWorks framing: "Those are security automation agents running in Falcon. We're talking about governing the AI agents your developers and business teams are deploying."
- SGNL capability is real: acknowledge it, then differentiate on AI agent lifecycle governance depth and MCP enforcement specifically

---

## Threat Assessment

**Where they win:** Existing Falcon customers wanting to extend the platform, SOC-centric buyers, EDR-first security orgs, endpoint detection use cases where behavioral anomaly matters more than governance.

**Where we win:** Identity-first buyers, governance-focused CISOs, on-prem requirements, coding agent session governance, MCP enforcement as prevention (not detection), purpose-built governance vs. EDR extension.

