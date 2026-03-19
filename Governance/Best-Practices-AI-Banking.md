# AI Governance Best Practices for Banking

This document provides high-level "Best Practices" for implementing AI agents within a financial services context, synthesized from industry leaders (AWS, Microsoft, Google, Databricks) and banking regulatory expectations (SR 11-7, CFPB).

---

## 🏗️ 1. Architecture & Security
- **Unified Governance:** Use a "single pane of glass" to govern both data and AI models. AI agents should automatically inherit the permissions and sensitivity labels of the data they access.
- **Data Lineage:** Maintain a clear audit trail of where training and prompt data comes from. For every AI output, you should be able to identify the "Source of Truth" document used.
- **PII/PHI Masking:** Implement real-time masking of sensitive customer data (SSNs, account numbers) *before* it is sent to a third-party LLM provider.

## ⚖️ 2. Risk Management & Compliance
- **Model Drift Monitoring:** Regularly test for "drift"—when an AI's accuracy or behavior degrades over time due to new data or model updates.
- **Explainability (XAI):** Ensure that every AI-driven decision (especially in credit or risk) can be explained in human-readable terms. "The model is too complex" is not a valid compliance defense.
- **Constitutional AI:** Give your agents a set of "Hard Rules" (a Constitution) that they must check against before generating any response.

## 👥 3. Operational Best Practices
- **Human-in-the-Loop (HITL):** Mandatory human sign-off for any action involving financial transfers, legal documentation, or customer-facing advice during the initial pilot phase.
- **Crawl-Walk-Run Approach:** Start with low-risk internal applications (e.g., policy search or meeting summarization) before moving to high-stakes client-facing or underwriting tasks.
- **Regression Testing:** Every agent update must undergo a full regression suite to ensure that "fixing" one capability hasn't broken another.

## 🌐 4. Digital Reputation Monitoring
- **Periodic Audits:** Regularly test how major LLMs perceive your organization by asking a standardized set of questions every 30 days. This tracks "digital reputation drift" and helps identify emerging risks.

---
**Status:** [ ] Draft | [ ] Approved by AI Committee
**Last Updated:** March 20, 2026
