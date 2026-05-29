# Battle Card: SentinelOne

**Last updated:** May 28, 2026
**Category:** Endpoint + Cloud + Identity Security (AI-native EDR platform)
**Ticker:** S
**Threat level:** MEDIUM-HIGH — strong endpoint heritage and genuine NHI detection capability. Prompt AI Agent Security adds MCP monitoring and real-time agent governance. Silverfort partnership extends NHI coverage. Weakest on governance workflows, lifecycle management, machine identity, and on-prem.

---

## What SentinelOne Claims

**Singularity Identity (NHI expansion, Feb 2026):**
- Secures human and non-human identities including AI agents
- Extends beyond authentication gatekeeping to runtime behavioral validation
- Continuous validation of intent through behavior — "authorization alone is not sufficient"
- Policy-based conditional access
- Silverfort partnership (Apr 2026): extends NHI coverage to MFA, lateral movement detection, and access management across hybrid environments

**Prompt AI Agent Security (GA RSA 2026):**
- Real-time discovery and governance control plane for AI agents
- Full MCP server visibility — discovers and monitors MCP servers across the environment
- Policy enforcement on agent behavior at runtime
- Extends Autonomous Security Intelligence into the agentic layer

**Detection Capability — Real Examples:**
- Detected and blocked Claude Code executing a malicious LiteLLM process chain (supply chain attack, March 2026)
- Behavioral validation that detects agents operating outside their defined function

**Silverfort Partnership:**
- Extends Falcon-style runtime protection to identity and NHI layer
- MFA extension to NHIs
- Access management across on-prem and cloud identity providers

---

## What They Actually Do (Honest Assessment)

SentinelOne is genuinely strong on endpoint security and behavioral detection. Their NHI expansion is real but carries the same architectural limitation as CrowdStrike: they are an EDR platform extending into identity, not an identity platform. Their MCP server visibility is real. Their behavioral detection for agent anomalies is real.

**What's real:**
- Prompt AI Agent Security has MCP server discovery and monitoring — GA at RSA 2026
- Behavioral validation extending beyond authentication is a genuine conceptual advance
- Detection of agent-related malicious activity (supply chain, process chain anomalies) is strong
- Silverfort partnership adds NHI MFA and access management depth

**What's weaker:**
- Governance workflows (ownership, lifecycle, onboarding/offboarding) are thin
- No MCP gateway — they monitor MCP activity, not intercept and enforce it
- No machine identity (CLM, PKI, certificates)
- No on-prem deployment for AI agent telemetry
- "Behavioral validation of agent intent" is aspirational positioning — the actual implementation is anomaly detection on top of endpoint telemetry, not true intent reasoning

---

## Where EOS Wins — The Genuine Gaps

### 1. Detection vs. Governance and Prevention
SentinelOne's core competency is detection and response — they are extremely good at finding bad things happening and stopping them. Their NHI and AI agent story is built on that foundation: detect anomalous agent behavior, respond, contain. The governance layer — defining what agents are allowed to do, who owns them, how they're provisioned and decommissioned — is not part of SentinelOne's architecture.

**Reframe:** "SentinelOne stops agents from doing bad things. EOS defines what agents are supposed to do in the first place. You need both — they don't overlap."

### 2. No MCP Gateway
SentinelOne monitors MCP servers — they have visibility into what MCP servers are operating and can detect anomalous tool invocations. They do not sit in the protocol path as a gateway that intercepts and enforces access policy per tool call. The same detect-vs-prevent distinction as Wiz and CrowdStrike.

**Reframe:** "SentinelOne sees what's happening in MCP sessions. EOS controls what's allowed to happen — per tool call, per agent, per session."

### 3. No Machine Identity
CLM, PKI, certificates, SSH — entirely outside SentinelOne's product scope. AppViewX + EOS spans from the cryptographic trust layer through AI agent runtime governance. SentinelOne addresses the endpoint and identity detection layer only.

### 4. Lifecycle Governance Gap
SentinelOne's identity platform is focused on runtime security — detecting and responding to identity attacks as they happen. There are no governance workflows for agent provisioning, ownership assignment, access reviews, or decommissioning. For compliance-focused buyers who need an audit trail of agent lifecycle from creation through retirement, SentinelOne's stack is incomplete.

### 5. On-Prem Agent Telemetry
SentinelOne is a cloud-native platform. Their Autonomous Security Intelligence and telemetry pipeline routes through their cloud. For buyers requiring agent telemetry to remain on-prem, SentinelOne has no answer. EOS deploys fully on-prem.

### 6. The Supply Chain Attack vs. Standing Privilege Distinction
SentinelOne's notable Claude Code detection (blocking a malicious LiteLLM process chain) is impressive — and it illustrates exactly what their platform is good at: detecting externally injected malicious behavior. The Broadridge problem is different: Claude Code is legitimate, authorized, and operating exactly as intended — with too much standing access. Behavioral anomaly detection cannot flag normal agent behavior that is over-permissioned. That requires a governance layer that defines expected behavior before the agent runs.

**Reframe:** "SentinelOne stopped an agent that was doing something malicious. EOS prevents an agent from doing something it was never supposed to be allowed to do — even if it's behaving normally."

---

## Common Objections and Responses

**"SentinelOne's behavioral validation goes beyond authentication — they validate intent."**
SentinelOne's "validation of intent through behavior" is really anomaly detection on top of endpoint and identity telemetry. They detect when an agent deviates from observed normal behavior. EOS defines expected behavior proactively through policy — what the agent is allowed to access, what tools it can invoke, what systems it can touch. Policy-driven prevention and behavioral anomaly detection are complements, not substitutes.

**"SentinelOne detected a real Claude Code attack in production — that's proven capability."**
The LiteLLM supply chain detection is real and impressive. That was a malicious code injection through a compromised package. The over-permissioned standing access problem at Broadridge is not detectable through behavioral anomaly — Claude Code accessing production systems with broad permissions looks identical to Claude Code accessing those systems with appropriate permissions. The distinction requires a policy layer, not a detection layer.

**"Silverfort partnership adds NHI coverage they didn't have before."**
True — Silverfort adds meaningful NHI access management depth to SentinelOne's platform. That partnership specifically helps with MFA extension to NHIs and lateral movement detection. It doesn't add agent lifecycle governance, MCP gateway enforcement, or machine identity.

**"SentinelOne has a perfect MITRE ATT&CK evaluation and Gartner Leader recognition."**
Six years as an EPP Magic Quadrant Leader is a real signal — for endpoint security. Their identity and NHI expansion is much newer. Evaluate AI agent governance on its own merits, separate from their endpoint excellence.

---

## The Positioning Line

SentinelOne is the best endpoint detection platform in the world. They are extending that detection capability into NHI and AI agent security. EOS is a governance and enforcement platform. Detection catches threats after they emerge. EOS prevents unauthorized behavior before it happens. Different layers, both necessary.

---

## Account Intel — When SentinelOne Is Already Deployed

- Strong on endpoint — don't compete there, position as additive
- Lead with governance layer: "SentinelOne protects your environment from bad actors. EOS governs what your AI agents are allowed to do so you don't create the problem in the first place."
- MCP gateway vs. MCP monitoring is the clearest technical distinction
- Machine identity is reliably outside their scope — strong cross-sell motion for AppViewX CLM
- On-prem requirement is an instant disqualifier
- Supply chain attack story is their best demo — use it to transition: "That was an external attacker. The Broadridge problem is an internal governance gap. Different problem, different tool."

---

## Threat Assessment

**Where they win:** Existing SentinelOne endpoint customers, SOC-centric buyers, environments where threat detection is the primary lens, attack detection and response use cases.

**Where we win:** Governance and prevention focus, machine identity, MCP gateway enforcement, agent lifecycle management, on-prem requirements, standing privilege elimination (as opposed to anomaly detection after the fact), compliance-driven audit trail requirements.

