---
name: follow-up-generator
description: Generate personalized follow-up emails and materials after client meetings
version: 1.0
status: planned
owner: Jason
category: post-meeting-analysis
tags: [follow-up, email, communication, client-engagement]
---

# Follow-Up Generator Agent

## Purpose
Automatically generate personalized, professional follow-up emails and supporting materials after client meetings, incorporating insights from transcript analysis.

## Capabilities

### 1. Email Composition
- Generate personalized greeting based on meeting tone
- Summarize key discussion points
- Confirm action items with clear ownership
- Include relevant attachments and resources
- Craft compelling call-to-action for next steps

### 2. Content Customization
- Adjust tone based on client relationship stage
- Incorporate client-specific terminology and references
- Match communication style to client preferences
- Include relevant case studies or resources

### 3. Multi-Format Output
- Standard follow-up email
- Executive summary attachment (PDF)
- Action item tracker (Excel/Google Sheets)
- Presentation materials referenced in meeting
- Technical documentation links

### 4. Strategic Elements
- Reinforce value propositions discussed
- Address concerns raised subtly
- Create urgency for next steps
- Build relationship through personalization

## Input Requirements
- Transcript analysis output (from transcript-analyzer agent)
- Meeting metadata and participant information
- Company email templates and branding guidelines
- CRM context (relationship history, preferences)
- Relevant resources and attachments

## Email Structure

```markdown
Subject: Following Up: [Personalized Topic] - [Next Action]

Hi [Name],

[Personalized opening referencing specific discussion point]

**Key Takeaways from Our Discussion:**
- [Insight 1 with specific reference]
- [Insight 2 with specific reference]
- [Insight 3 with specific reference]

**Action Items & Next Steps:**

On Our Side:
- [ ] [Action item] - [Owner] - Due: [Date]
- [ ] [Action item] - [Owner] - Due: [Date]

On Your Side:
- [ ] [Action item] - [Contact] - Due: [Date]

**Resources & Materials:**
- [Relevant document/link with context]
- [Case study or white paper]

**Proposed Next Steps:**
[Specific call-to-action with proposed date/time]

[Warm, personalized closing]

Best regards,
[Signature]

---
[Company footer with contact info]
```

## Guardrails
- **Accuracy Check:** Flag any claims not substantiated in transcript
- **Tone Analysis:** Ensure appropriate formality level
- **Compliance Review:** No unauthorized commitments
- **Privacy:** Remove internal-only information
- **HITL Approval:** Sales rep reviews before sending

## Integration Points
- **Input:** transcript-analyzer agent output
- **CRM:** Pull client preferences and history
- **Email System:** Draft in Gmail/Outlook
- **Calendar:** Suggest meeting times via Calendly
- **Document Storage:** Attach from SharePoint/Google Drive
- **Analytics:** Track email opens and engagement

## Workflow

```yaml
workflow:
  1_analyze_input:
    - Receive transcript analysis
    - Extract action items and key points
    - Identify tone and relationship stage

  2_draft_generation:
    - Select appropriate template
    - Personalize content
    - Add relevant resources
    - Structure action items

  3_quality_checks:
    - Accuracy validation
    - Compliance screening
    - Grammar and tone check
    - Link verification

  4_hitl_review:
    - Send to meeting owner for review
    - Accept feedback and revisions
    - Approve for sending

  5_delivery:
    - Send via email client
    - Log in CRM
    - Schedule follow-up reminder
    - Track engagement metrics
```

## Success Metrics
- Time saved per follow-up (target: 85% reduction)
- Email response rate (track engagement)
- Action item completion rate
- Client satisfaction scores
- Sales velocity improvement

## Personalization Engine

### Client Relationship Stage
- **First Meeting:** More formal, educational focus
- **Active Deal:** Action-oriented, deadline-driven
- **Long-term Client:** Friendly, strategic partnership tone
- **Renewal Discussion:** Value reinforcement, relationship building

### Industry Customization
- **Banking/Finance:** Emphasize compliance and security
- **Technology:** Highlight innovation and integration
- **Healthcare:** Focus on privacy and regulatory alignment
- **Government:** Stress transparency and accountability

## Template Library
```yaml
templates:
  - name: "discovery-follow-up"
    use_case: "First discovery meeting"
    tone: "Professional, exploratory"

  - name: "technical-deep-dive"
    use_case: "Technical validation meeting"
    tone: "Detailed, technical"

  - name: "executive-alignment"
    use_case: "C-level strategic discussion"
    tone: "Concise, high-level, strategic"

  - name: "proposal-submission"
    use_case: "Following proposal presentation"
    tone: "Confident, action-oriented"
```

## Next Steps
- [ ] Build template library with sales team input
- [ ] Integrate with transcript-analyzer agent
- [ ] Create HITL review interface
- [ ] Establish A/B testing for email effectiveness
- [ ] Connect to CRM for engagement tracking
- [ ] Build analytics dashboard for follow-up performance
