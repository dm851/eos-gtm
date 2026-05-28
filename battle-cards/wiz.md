# Battle Card: Wiz (AI-APP)

**Last updated:** May 28, 2026  
**Category:** Cloud Security / CNAPP expanding into AI application security  
**Owned by:** Google (acquired March 2026, $32B)  
**Threat level:** HIGH — dominant distribution, Fortune 100 penetration, bundling risk

---

## What Wiz Claims

Wiz launched the **AI Application Protection Platform (AI-APP)** in March 2026, positioned as CNAPP evolved for AI. Their messaging covers:

- Full-stack AI inventory (AI-BOM): models, agents, tools, IDE extensions, MCP servers
- Risk analysis across infrastructure + data + model + agent layers via the Security Graph
- Runtime threat detection via eBPF sensor + cloud telemetry (Wiz Defend)
- Wiz Code: IDE plugins for Claude Code, Cursor, VS Code, JetBrains — pre-commit scanning
- AI-SPM: posture management across managed services (Bedrock, Vertex, Azure AI) and SaaS AI platforms
- Three internal AI agents: Red (attacker simulation), Green (remediation), Blue (investigation)
- Partnership with Saviynt for NHI and AI agent lifecycle governance (announced Feb 2026)
- Integration with Google Cloud's Agent Gateway (MCP/A2A protocol inspection) at Cloud Next '26

---

## What Wiz Actually Does (vs. What They Claim)

| Claim | Reality |
|---|---|
| "Runtime enforcement" | Runtime **detection** via eBPF + cloud telemetry. Observes and alerts. Does not block agent actions before they execute. |
| "Agent governance" | Posture management and risk scoring. Lifecycle governance (ownership, onboarding, offboarding) is handled by Saviynt via a partnership — not native to Wiz. |
| "MCP security" | Wiz has MCP security content (blog, academy). Agent Gateway (Google Cloud) inspects MCP/A2A traffic but is a Google infrastructure product — not Wiz enforcing agent-level access policy. |
| "Coding agent security" | IDE plugins catch hardcoded secrets, IaC misconfigs, and vulnerable dependencies at pre-commit. Does not govern what the agent accesses at runtime during an active session. |
| "AI agent inventory" | Strong for cloud-native and managed platform agents (Bedrock, Copilot Studio). Weaker for on-prem, custom homegrown platforms with no cloud API surface. |

---

## Where Wiz Has Real Coverage (Be Honest)

- Cloud infrastructure posture for AI workloads: strong
- AI-BOM / shadow AI discovery across managed services and SaaS: strong
- Attack path analysis connecting infra + identity + data + AI layers: strong
- Pre-commit scanning for coding agent-generated code: real and improving
- Prompt injection awareness in code (SAST rules, OWASP LLM Top 10 mapping): real
- Distribution and install base: dominant — 50%+ of Fortune 100

---

## Where EOS Wins — The Genuine Gaps

### 1. Enforce vs. Detect
Wiz detects bad outcomes after they occur or identifies risk posture proactively. EOS enforces policy at the moment of execution — the agent's action is blocked before it completes. The PocketOS scenario (Cursor deleting a production DB) is not preventable by Wiz. Cursor was doing exactly what it was designed to do, with access it legitimately had. No cloud telemetry would have flagged it until after the database was gone.

**Reframe:** "Wiz tells you what happened. EOS governs what's allowed to happen."

### 2. Developer Endpoint Blind Spot
Wiz's runtime layer watches cloud telemetry and workload execution at the infrastructure layer. Coding agent sessions (Claude Code, Cursor) run on developer endpoints, inside a local IDE session, before anything touches a cloud API or gets committed. That activity is invisible to Wiz. EOS's agent sensor operates at the endpoint, in the session, where the risk actually lives for the coding agent use case.

**Reframe:** "If your coding agent accesses a production system during an active dev session and nothing gets committed, Wiz never saw it."

### 3. No Native Governance Layer
Wiz has no agent ownership model, no lifecycle workflows (onboarding/offboarding/transfer), no policy engine defining what an agent is permitted to do. Their answer to governance is a partnership with Saviynt — a separate product, separate contract, separate deployment. EOS governs agent identity natively: ownership assignment, access policy, JIT provisioning, lifecycle management.

**Reframe:** "Wiz + Saviynt is two products stitched together. EOS is one governance layer."

### 4. No MCP Gateway
Wiz does not have an MCP gateway product. Agent Gateway is a Google Cloud infrastructure product — not a Wiz product. It inspects MCP traffic in Google Cloud environments only. It does not enforce agent-level access policy across platforms. EOS's MCP gateway sits in front of any MCP server, enforces JIT access, eliminates standing privileges, and logs every tool call regardless of which cloud or platform the agent runs on.

**Reframe:** "Google's Agent Gateway secures MCP traffic in GCP. EOS's MCP gateway secures agent access everywhere — cloud, on-prem, multi-platform."

### 5. On-Prem Is a Non-Starter for Wiz
Wiz is SaaS-native, agentless via cloud API. Their own documentation acknowledges agentless tools are "less effective for on-premises hosts." For security-conscious CISOs who will not allow agent telemetry to leave their environment — Broadridge, ZoomInfo, Freshworks, DocuSign, JB Poindexter — Wiz has no answer. EOS deploys on-prem by design.

**Reframe:** "For any buyer who needs agent telemetry to stay inside their environment, Wiz is not an option."

### 6. Cloud-Native Bias = Vendor Lock-in Risk
Wiz is now Google. Their agent governance roadmap runs through Google Cloud Agent Gateway, Google Security Operations (Chronicle), and the Google Gemini Enterprise Agent Platform. Enterprises running multi-cloud or non-GCP environments should ask how neutral Wiz's coverage remains under Google ownership. EOS is cloud-agnostic by design.

---

## Common Objections and Responses

**"We already have Wiz. Does EOS overlap?"**  
Some overlap on discovery and inventory — both build an AI bill of materials. But Wiz does not govern what agents are allowed to do, does not enforce runtime policy, does not manage agent lifecycle, and does not have an MCP gateway. If your Wiz deployment tells you what AI agents exist, EOS tells them what they're allowed to do. These are complementary layers, not substitutes.

**"Wiz has runtime protection."**  
Wiz has runtime detection — eBPF sensor and cloud telemetry that alert on anomalies after they occur. EOS has runtime enforcement — policies that block unauthorized agent actions before they execute. Detection and prevention are not the same capability. If an agent deletes a production database, Wiz logs the cloud activity. EOS blocks the action.

**"Wiz has coding agent security via IDE plugins."**  
Wiz Code plugins catch insecure code before it's committed — hardcoded secrets, IaC misconfigs, vulnerable dependencies. That's a supply chain / AppSec control. It does not govern what the coding agent accesses during an active session. If Claude Code reads a production config file or calls a sensitive API in the middle of a session, pre-commit scanning missed it entirely.

**"Doesn't CI/CD catch this?"**  
CI/CD pipeline scanning catches artifacts that pass through the pipeline: committed code, IaC templates, container images. Coding agent sessions that access production systems directly — without committing anything — never enter a pipeline. The PocketOS incident was a live session action, not a pipeline artifact.

**"Wiz partnered with Saviynt for agent governance."**  
Yes, which means Wiz acknowledged they do not have native agent governance. The Saviynt integration adds lifecycle management and ownership association via a separate product. That is a two-vendor, two-contract, two-deployment answer to a problem EOS solves natively.

---

## The Positioning Line

Wiz is a cloud security company adding AI coverage. EOS is a governance platform purpose-built for the AI agent identity problem. Wiz sees what your agents are doing in the cloud. EOS controls what they are allowed to do — anywhere.

---

## Account Intel — When Wiz Is Already Deployed

If Wiz is in the account:
- They are likely already doing AI-BOM / shadow AI discovery — don't compete on that
- Lead with governance, lifecycle, and enforcement — the three things Wiz does not natively do
- Ask: "What happens when Wiz identifies an over-permissioned agent? Who defines the policy? How do you enforce it?" There is no Wiz answer to that without Saviynt
- For on-prem requirements: immediate disqualifier for Wiz
- For coding agent endpoint coverage: Wiz's pre-commit plugin is not the same as session-level enforcement. Ask about the session gap.

---

## Wiz Threat Assessment

**Where they win:** Cloud-native accounts, GCP-heavy environments, accounts already using Wiz CNAPP who want to extend coverage without a new vendor. Strong with AppSec and cloud security teams. Google distribution is formidable.

**Where we win:** Identity-first buyers (CISO, Head of Security Architecture), on-prem requirements, coding agent governance (endpoint session level), governance-and-lifecycle buyers, multi-cloud / non-GCP accounts wary of Google lock-in, regulated industries needing strict audit trail and policy enforcement — not just posture visibility.

**The bundling risk:** Wiz will try to consolidate AI security alongside CNAPP in existing accounts. The counter is depth — Wiz is wide, EOS is deep on governance and enforcement. Position as the identity governance layer that makes Wiz findings actionable.

