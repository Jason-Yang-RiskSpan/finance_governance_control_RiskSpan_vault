# Team AI Strategy & Control Plane Index

This document summarizes the core vision and internal requirements shared by Dan and Pat for our AI agent ecosystem, specifically the development of an **Agent Control Plan** and our **Governance/Audit** standards.

---

## 🏛 1. The Agent Control Plan (Command Hub)
The central component for managing AI agents and telemetry.
- **Infrastructure:** Dedicated consulting repo, individual enterprise IDs, and managed backend.
- **Governance:** 
    - Every agent requires explicit permissions, a testing suite, and guardrails.
    - **Observability Agent:** Proposed by Jason to increase transparency during deployment.
- **Audit Trails:** All logs must be saved within the backend instance for violation querying.

## ⚖️ 2. Regulatory & Governance Frameworks
How our internal agents align with global banking standards.
- [[Governance/Frameworks/SR 11-7 - Model Risk Management|SR 11-7: Model Risk Management]]
- [[Governance/Frameworks/CFPB - AI Explainability Requirements|CFPB: Explainability & Anti-Bias]]
- [[Governance/Frameworks/Third-Party AI Risk|Third-Party AI & Vendor Governance]]
- **Regulatory Agent:** Planned tool to monitor Singapore, Korea, and EU updates.

## 📊 3. Audit, Reporting & "RS Verify"
Monthly technical and executive reports covering:
- Model drift and infrastructure optimization.
- Token usage and improvement suggestions.
- **Digital Presence Assessment:** Grading company reputation across 5 major LLMs with 21 questions every 30 days.

## 🔄 4. Automated Workflows (Agent Skills)
Current and planned skills for our local cloud instance:
- **Pre-Discovery:** Market research, meeting scripts, and agenda generation.
- **Post-Meeting:** Transcript analysis against policy and automated follow-up actions.
- **JIRA Integration:** Automated ticket creation in the improvement loop.

## 🛡 5. Core Client Requirements
- **Accountability:** Clear ownership of every agent action.
- **Assurance:** Verified testing and regression suites for every agent.
- **Human Oversight:** Mandatory "Human-in-the-Loop" during initial deployment phases.

---
**Key Contacts:** Dan, Pat, Jason, Honghua, Jungmo
**Status:** In Development (Infrastructure Setup Phase)

## Sources & References
*   **Framework:** [NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/itl/ai-risk-management-framework)
*   **Banking Guidance:** [SR 11-7: Guidance on Model Risk Management](https://www.federalreserve.gov/supervisionreg/srletters/sr1107.htm)
