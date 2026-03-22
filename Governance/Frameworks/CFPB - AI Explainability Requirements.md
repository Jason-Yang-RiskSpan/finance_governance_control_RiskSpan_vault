# CFPB - AI Explainability Requirements

**Primary Agency:** Consumer Financial Protection Bureau (CFPB)
**Key Regulations:** Equal Credit Opportunity Act (ECOA) / Regulation B

## Core Requirement: Explainability

The CFPB has issued circulars (2022-03 and 2023-03) clarifying that "the AI was too complex to explain" is **not a valid legal defense** for failing to provide an accurate Adverse Action Notice.

### Adverse Action Notices
*   **Specific Reasons:** If a credit application is denied, the bank must provide the *top specific reasons* for the denial.
*   **Accuracy:** The reasons provided must be the *actual* factors that the model used to make the decision.
*   **Anti-Bias Monitoring:** Models must be tested for "algorithmic redlining" (e.g., a model using zip codes as a proxy for race).

### Governance Checklist for Explainable AI (XAI)
*   [ ] Does the model's documentation specify the top 5-10 driving variables?
*   [ ] Is there a process to translate complex model outputs into human-readable reasons for consumers?
*   [ ] Have fair-lending tests (e.g., disparate impact analysis) been performed on the model?

---
**Status:** [ ] To Review | [ ] In Compliance

## Sources & References
*   **CFPB Circular 2022-03:** [Adverse Action Notification Requirements (Complex Algorithms)](https://www.consumerfinance.gov/compliance/circulars/circular-2022-03-adverse-action-notification-requirements-in-connection-with-credit-decisions-based-on-complex-algorithms/)
*   **CFPB Circular 2023-03:** [Adverse Action Notification Requirements (Sample Forms & Data Use)](https://www.consumerfinance.gov/compliance/circulars/consumer-financial-protection-circular-2023-03-adverse-action-notification-requirements-and-the-proper-use-of-the-cfpbs-sample-forms-provided-in-regulation-b/)
