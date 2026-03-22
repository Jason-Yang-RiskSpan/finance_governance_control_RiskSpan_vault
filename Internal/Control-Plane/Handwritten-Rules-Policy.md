# Handwritten Rules & Policy Document (V1.0)

**Status:** Under Review - Last Updated: March 20, 2026
**Owner:** Dan / Pat
**Contributors:** Jason (Observability / Improvement Suggestions)

## ⚖️ Core Mission Statement
Our AI agents are built to provide **Accountability** and **Assurance** to our clients. Every action taken by an agent must be reversible, documented, and aligned with our internal safety and performance standards.

---

## 🏛️ Rule 1: Infrastructure & Control Plane
- Every AI agent MUST have an enterprise-level parent instance with role-based derivatives for team members.
- Agents CANNOT operate outside of the managed cloud code repository without explicit approval.
- All agent telemetry (prompts, logs, and reasoning) MUST be persisted in the backend instance for audit querying.

## 🛡️ Rule 2: Governance & Guardrails
- **Human Oversight:** High-risk financial or operational actions MUST have a "Human-in-the-Loop" sign-off during initial deployment.
- **Permissions:** Agents MUST operate within explicit permission boundaries. Any attempt to bypass guardrails (e.g., via "Mole Book" style techniques) must be flagged and logged.
- **Audit Requirement:** Every agent requires a documented sign-off on its testing suite and guardrails before it is promoted to production.

## 🔄 Rule 3: Improvement & Iteration
- **Regression Testing:** Each agent must have an attached test regression suite. An overarching regression suite MUST run weekly checks across the entire ecosystem.
- **JIRA Integration:** Agents must be configured to automatically create JIRA tickets for bug fixes or infrastructure improvements in their own "improvement loop."
- **RS Verify:** Agents' performance will be reviewed monthly via the "RS Verify" product, focusing on model drift, token usage, and cost-to-value optimization.

## 📊 Rule 4: Digital Reputation
- Every 30 days, we will audit five leading LLMs by asking 21 predefined questions to assess and grade the company's digital presence and reputation.

---
**Next Actions:**

## Sources & References
*   **Policy Framework:** [NIST AI RMF - Govern Function](https://www.nist.gov/itl/ai-risk-management-framework)
*   **Responsible AI:** [Microsoft Responsible AI Standard](https://www.microsoft.com/en-us/ai/responsible-ai)
- [ ] Finalize the "RS Consulting" infrastructure policy.
- [ ] Review the "Code Repository" access permissions with Pat.
- [ ] Integrate JIRA / Azure ticket automation protocols.
