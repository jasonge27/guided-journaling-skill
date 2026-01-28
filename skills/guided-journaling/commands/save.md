# Save Command

## Trigger

User types `/save` or asks to save the session.

## Process

1. Review the entire conversation
2. Generate the three-section session record
3. Write to `sessions/session_YYYY-MM-DD_journal.md`
4. If file exists, append `_2`, `_3`, etc.

## Output Template

```markdown
# Session: YYYY-MM-DD

## 1. High-Level Summary

- **Date/Time**: YYYY-MM-DD (Day of week), [morning/afternoon/evening if known]
- **Mode**: [cbt/reflective/relationship/mixed]
- **Duration**: [approximate based on exchange count]
- **Key People**: [names mentioned with brief identifier, e.g., "Alex (partner)", "Mom"]
- **Key Events**: [bullet list of events discussed]
- **Locations**: [places mentioned if relevant]
- **Primary Emotions**: [emotions expressed: anxiety, sadness, frustration, etc.]
- **Core Insights**: 
  - [Insight 1 - one sentence]
  - [Insight 2 - one sentence]
- **Patterns Identified**: [new or reinforced patterns]
- **Action Items**: [what user plans to do, if any]
- **Follow-up Topics**: [threads to revisit next time]

---

## 2. Detailed Summary

### Arriving State
[How the user arrived emotionally, what prompted the session]

### Session Arc
[Narrative of what was explored, in order]

### Key Therapeutic Moments
[Specific breakthroughs, reframes, or insights with context]

### Patterns & Themes
[How this session connects to ongoing patterns from previous sessions]

### Closing State
[Where the user landed emotionally, any shifts from start]

### Unfinished Business
[Topics that need more exploration, questions left hanging]

---

## 3. Complete Transcript

### Exchange 1
**User**:
[Exact text of user's message]

**Assistant**:
[Exact text of assistant's response]

---

### Exchange 2
**User**:
[Exact text]

**Assistant**:
[Exact text]

---

[Continue for all exchanges...]

---

*Session saved: YYYY-MM-DD HH:MM*
```

## Guidelines

### High-Level Summary
- Keep it scannable—for quick pattern-matching across sessions
- Include ALL people mentioned by name
- Emotions should be specific (not just "bad" but "anxious, trapped, frustrated")
- Core insights should be quotable—the "aha" moments

### Detailed Summary
- Write as narrative, not bullet points
- Include enough context that someone reading only this section understands the session
- Note which therapeutic techniques were used
- Explicitly connect to previous sessions when relevant

### Complete Transcript
- **Verbatim**—do not summarize or edit
- Include the assistant's full responses, not shortened versions
- Preserve formatting (line breaks, emphasis, etc.)

## Example High-Level Summary

```markdown
## 1. High-Level Summary

- **Date/Time**: 2026-01-12 (Monday), evening
- **Mode**: relationship + reflective
- **Duration**: ~6 exchanges, medium session
- **Key People**: Alex (partner), Sarah (friend)
- **Key Events**: 
  - Conflict with partner about upcoming travel plans
  - Difficult conversation about needs and boundaries
  - Processing work stress
- **Locations**: Home, mentioned upcoming trip
- **Primary Emotions**: frustrated, trapped, drained, anxious
- **Core Insights**: 
  - "I feel suffocated because expressing my need for space gets heard as rejection"
  - "I'm evaluating whether my reasons are 'good enough' to have needs—but needing space IS a valid reason"
- **Patterns Identified**: 
  - NEW: Pursue-withdraw dynamic with partner
  - REINFORCED: Difficulty expressing needs
  - NEW: "Must have sufficient reason to deserve having needs"
- **Action Items**: None explicit—user too depleted
- **Follow-up Topics**: 
  - Does partner know how suppressed they feel?
  - Processing difficult memories associated with certain places
  - Partner's possible separation anxiety
```

## After Saving

Confirm to user:
- File location
- Brief summary of what was captured
- Invitation for next session
