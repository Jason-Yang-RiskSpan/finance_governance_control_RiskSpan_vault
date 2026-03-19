# AI Model Validation Checklist

**Source:** Based on NIST AI RMF and SR 11-7

Use this checklist during the **Independent Model Validation** phase.

### Phase 1: Conceptual Soundness
*   [ ] Does the model have a clear and valid business objective?
*   [ ] Is the math/logic used by the model appropriate for the financial problem it solves?
*   [ ] Are the training data sources clearly documented and representative?

### Phase 2: Performance & Outcome Testing
*   [ ] Have we tested the model's accuracy on out-of-sample data?
*   [ ] Does the model's performance "degrade" significantly under stress (e.g., market volatility)?
*   [ ] Have we identified the "failure modes" where the AI provides confidently wrong answers?

### Phase 3: Fairness & Anti-Bias
*   [ ] Has a Disparate Impact Analysis been completed for all protected classes?
*   [ ] Does the model unintentionally use "proxy variables" (e.g., education level as a proxy for socioeconomic status)?

### Phase 4: Operational Controls
*   [ ] Is there a "Human-in-the-Loop" (HITL) process for high-risk decisions?
*   [ ] Is there an automated "Model Drift" alert system?
*   [ ] Has the Board of Directors/Risk Committee approved this model for deployment?

---
**Status:** [ ] Draft | [ ] Final
