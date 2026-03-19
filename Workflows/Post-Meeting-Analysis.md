# Post-Meeting Analysis Workflow

**Goal:** Automate the processing of meeting transcripts to ensure compliance, generate follow-up actions, and provide strategic improvement suggestions.

## 📋 Process Overview
This workflow runs after every major client meeting or internal pre-discovery session.

### Phase 1: Data Ingestion & Synthesis
- **Input:** Meeting transcripts (from Zoom/Teams/etc.) and shared documents.
- **Agent Skill:** Synthesize the primary themes, key decisions, and "implicit" client needs not stated in the transcript.

### Phase 2: Compliance & Policy Analysis
- **Audit Against Policy:** The agent compares the transcript against our internal governance and risk policies.
- **Violation Checks:** Flag any instances where an agent or representative may have overstepped their authority or misaligned with the RS Verify standards.

### Phase 3: Actionable Output Generation
- **Follow-up Actions:** Generate a draft email for the project manager with clear next steps.
- **JIRA Integration:** Automatically create tickets for any infrastructure improvements or code changes identified during the meeting.
- **Improvement Suggestions:** The agent provides "Strategic Feedback" (e.g., "The client seemed hesitant about the Control Plane's transparency; consider emphasizing the Observability Agent in the next pitch.").

## 🛠 Required Skills & Tools
- **Transcript Processor:** High-context LLM capable of analyzing 1+ hour long meetings.
- **Policy Engine:** A database of current "Handwritten Rules" and policies for the agent to reference.
- **Connector:** Integration with the Agent Control Plane for task dispatching.

---
**Status:** [ ] Draft | [ ] Beta Testing
**Next Steps:**
- [ ] Connect this workflow to the JIRA automation loop.
- [ ] Define the "Policy Library" for the agent to use as a baseline.
