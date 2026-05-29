# Battle Card: Okta

**Last updated:** May 28, 2026
**Category:** Identity Platform (Workforce + Customer + AI Agent)
**Ticker:** OKTA
**Threat level:** HIGH on agent registration and directory-based governance. Massive install base. Weakest on NHI posture management, machine identity, MCP gateway, coding agent governance, and on-prem.

---

## What Okta Claims

**Okta for AI Agents (GA April 30, 2026):**
- Discover and register known and unknown AI agents into the Okta Universal Directory
- Treat agents as first-class identities — same directory, same governance model as humans
- Standardize agent access using short-lived tokens and scoped authentication
- Instant revocation of agent access (kill switch) for rogue agent behavior
- Governance for agents as a resource: automated access reviews, ownership assignment, policy enforcement
- Audit trail via system logs: agent activity, tool calls, authorization decisions sent to SIEM
- Certified access reviews and certification workflows
- Integration with Amazon Bedrock AgentCore for agent lifecycle management
- Works with any identity provider

**Framework — Three Questions:**
1. Where are my agents?
2. What can they connect to?
3. What can they do?

**Okta Identity Governance (existing):**
- Certification workflows, access reviews, separation of duties
- Now extended to AI agents as a governed resource type

---

## What They Actually Do (Honest Assessment)

Okta's approach is the most IAM-native of all competitors. They are treating AI agents like a new type of user in the directory — assigning them identities, governing their access through standard Okta workflows, and extending existing governance mechanisms to cover them.

**What's real:**
- Agent registration and directory-based identity is genuine and shipping
- Short-lived token provisioning for agents is a real capability
- Universal logout / kill switch for immediate access revocation is strong
- Okta's install base is massive — if a customer already uses Okta for workforce identity, adding agents to the same governance model is low friction
- Access reviews and certification workflows extended to agents are real

**What's missing:**
- No MCP gateway or protocol-level enforcement
- No behavioral anomaly detection for NHIs (not an Okta competency)
- No machine identity (CLM, PKI, certificates, SSH) — entirely orthogonal to Okta's product history
- No coding agent endpoint session governance
- No on-prem deployment for agent telemetry
- Governance model is IAM-native (directory, access reviews, certification) — not designed for the ephemeral, autonomous, non-deterministic behavior of AI agents

---

## Where EOS Wins — The Genuine Gaps

### 1. IAM Model Applied to an Agent Problem
Okta's governance model was designed for human users. Agents are registered in the directory, given identities, and governed through certification workflows — the same model used for a new employee. The problem: AI agents don't behave like employees. They spin up and down in milliseconds, take non-deterministic actions, operate across multiple systems simultaneously, and can't be governed by a quarterly access review. Static, directory-based governance is insufficient for a dynamic, autonomous agent.

**Reframe:** "Okta registers agents in a directory and runs access reviews. EOS governs what agents actually do at runtime — per session, per tool call, in real time. A quarterly certification workflow cannot stop an agent from deleting a production database this afternoon."

### 2. No MCP Gateway or Protocol-Level Enforcement
Okta has no MCP gateway. They govern agent access at the identity layer — what an agent is allowed to authenticate to. Once the agent is authenticated and operating, Okta has no visibility into what tool calls it makes through MCP, what files it reads, or what APIs it invokes. EOS's MCP gateway sits in the protocol path and enforces policy at the moment of every tool call.

**Reframe:** "Okta controls the door — who gets in. EOS controls what they're allowed to do once inside."

### 3. No Machine Identity
Okta has never played in machine identity, CLM, or PKI. This is entirely outside their product scope. For enterprise buyers who need to solve the 90-day TLS mandate, PQC migration, and AI agent governance simultaneously, Okta cannot be the answer. AppViewX + EOS is the only unified platform.

### 4. No NHI Posture or Behavioral Detection
Okta's approach to NHI is directory-based governance — assign it an identity, run access reviews. They have no behavioral anomaly detection for NHIs, no secret rotation, no secrets posture management. For buyers who want to understand NHI risk posture (over-permissioned service accounts, orphaned identities, credential sprawl), Okta is not the tool.

### 5. On-Prem Non-Starter
Okta is SaaS-only. For financial services, healthcare, or regulated industries with hard on-prem requirements, Okta's agent governance story ends there. EOS deploys fully on-prem.

### 6. Coding Agent Governance Gap
Okta's model registers agents that are known and formally provisioned through IT workflows. Shadow coding agents — developers standing up Claude Code or Cursor on their laptops — are not going through an Okta onboarding flow. Entro's EDR-based discovery or EOS's agent sensor discovers these. Okta's directory only knows what was registered.

---

## Common Objections and Responses

**"We already use Okta. Can't we just add agents to the directory?"**
You can register known agents in Okta — and you should, for the ones you know about. The problem is: registration doesn't govern runtime behavior. Once an agent is registered and authenticated, Okta has no control over what it does. And shadow agents — Claude Code on a developer laptop, a Cursor session accessing production — will never go through an Okta registration flow. EOS discovers them all, governs their access, and enforces policy at runtime.

**"Okta for AI Agents went GA in April — they're ahead of most vendors."**
First mover matters less than the right architecture. Okta shipped a directory-based governance model for a dynamic, ephemeral, autonomous identity class. The model is familiar (good) but fundamentally mismatched to the behavioral characteristics of AI agents (bad). Getting there first with the wrong architecture is a liability when buyer sophistication increases.

**"Okta's kill switch for instant revocation is a strong safety feature."**
It is — instant revocation is genuinely valuable for rogue agent response. EOS also has access revocation, plus the MCP gateway to prevent unauthorized actions before they require revocation. Prevention is a better outcome than revocation after the fact.

**"Our CISO wants everything through Okta for governance consistency."**
Governance consistency is a valid goal. The counter: Okta can govern who your agents are. EOS governs what they do. Both are necessary for a complete governance posture. They don't overlap — they stack.

---

## The Positioning Line

Okta assigns agents an identity in the directory. EOS governs what they actually do with it — per session, per tool call, in real time at the MCP gateway and developer endpoint. Identity registration and runtime governance are different layers. Both are necessary.

---

## Account Intel — When Okta Is Already Deployed

- Position as complementary: Okta handles workforce identity governance; EOS handles agent runtime enforcement and machine identity
- Lead with MCP gateway and coding agent endpoint coverage — both outside Okta's scope
- Machine identity gap is reliable — CLM/PKI is entirely orthogonal to Okta
- On-prem requirement is an instant disqualifier
- Okta's model works for formally provisioned agents — lead with shadow coding agent discovery as the gap Okta can't see

---

## Threat Assessment

**Where they win:** Existing Okta workforce customers wanting to extend governance to known agents, IT-governed AI deployments, formal agent registration workflows, access review and certification use cases.

**Where we win:** Runtime enforcement, MCP gateway, machine identity, shadow agent discovery, coding agent endpoint governance, on-prem deployment, behavioral governance vs. directory governance, ephemeral and autonomous agent populations that don't fit a directory model.

