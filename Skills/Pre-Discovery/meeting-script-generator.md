---
name: meeting-script-generator
description: Generate customized meeting agendas and talking scripts for client discovery sessions
version: 1.0
status: planned
owner: Jason
category: pre-discovery
tags: [meetings, scripts, agenda, discovery]
---

# Meeting Script Generator

## Purpose
Automatically generate customized meeting agendas, scripts, and discussion guides for client discovery sessions based on market research and client profile.

## Capabilities

### 1. Agenda Generation
- Create structured meeting agendas with time allocations
- Incorporate client-specific topics and pain points
- Include ice-breakers and relationship-building elements
- Add technical deep-dive sections as needed

### 2. Script Development
- Generate opening statements and introductions
- Create question frameworks for discovery
- Develop transition statements between topics
- Prepare closing summaries and next-step outlines

### 3. Personalization
- Tailor content to client industry and maturity level
- Adjust technical depth based on audience
- Include client-specific references and examples
- Incorporate previous interaction history

### 4. Supporting Materials
- Generate slide deck outline
- Create handout summaries
- Prepare demo scenarios
- Develop follow-up email templates

## Input Requirements
- Market research report (from market-research agent)
- Client profile and history
- Meeting objectives and goals
- Participant list and roles
- Time constraints and format (virtual/in-person)

## Output Format
```yaml
meeting_agenda:
  duration: 60 minutes
  participants: [list]
  objectives: [list]

sections:
  - title: "Opening & Introductions"
    duration: 5 minutes
    script: |
      [Detailed talking points]

  - title: "Current Challenges Discovery"
    duration: 20 minutes
    key_questions:
      - [Question 1]
      - [Question 2]

  - title: "Solution Overview"
    duration: 25 minutes

  - title: "Next Steps & Close"
    duration: 10 minutes

follow_up:
  - [Action items]
```

## Guardrails
- Flag any claims requiring verification
- Ensure compliance with company messaging guidelines
- Avoid over-promising capabilities
- Maintain professional and inclusive language

## Integration Points
- Receives input from market-research agent
- Connects to presentation generator
- Links to CRM for meeting logging
- Feeds into Post-Meeting-Analysis workflow

## Success Metrics
- Meeting effectiveness ratings from sales team
- Time saved in meeting preparation (target: 70%)
- Conversion rate from discovery to proposal

## Next Steps
- [ ] Create meeting template library
- [ ] Integrate with market-research agent output
- [ ] Establish review process with sales leadership
- [ ] Build feedback loop for continuous improvement
