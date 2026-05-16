---
type: status_update_lateral
form: artifact
register: direct, diagnostic
audience: peers, cross-functional partners, adjacent leadership
when_to_use: >
  Weekly or periodic status artifact distributed to peers and cross-functional
  partners who need situational awareness on your teams' delivery, operations,
  and risk posture. This is not a message — it is a document. The message that
  distributes it is an artifact_broadcast. Originally designed as private 1:1
  prep for SEM conversations; now shared broadly because peers found the signal
  useful. The public version omits personnel details (performance conversations,
  personal disclosures, private coaching context).
---

## What This Is

The SEM report is the primary instance of `status_update_lateral` in Joe's
communication system. It is generated weekly by the V2 pipeline and distributed
to peers who want the same delivery/operations picture Joe uses for his 1:1s.

The report has two versions:
- **Private (1:1 prep):** Full detail including suggested questions, personnel
  context, and coaching observations. Not distributed.
- **Public (lateral distribution):** Same delivery and operations data, suggested
  questions removed or reframed, personnel details stripped.

The template below describes the public version — the one that travels laterally.

---

## Structural Pattern

The document has six sections, always in this order:

1. **What Decisions Is Telling Me** — the SEM's own voice: their card submission,
   top priorities, highlights, lowlights, blockers, management asks. If no card
   was submitted, say so explicitly. Do not infer or substitute.

2. **Changes This Week** — week-over-week deltas only. Delivery date shifts,
   ETRC score changes, significant velocity moves. No narrative — just the delta
   and the direction. If nothing changed, say "No significant changes this week."

3. **Delivery Health** — table per team: version, planned date, projected date,
   status emoji, completion percentage. Follow with impacted epics for any
   at-risk or late team. The table is the signal; the epic list is the evidence.

4. **Time Allocation** — hours by epic, work type breakdown (Feature / Tech Debt /
   Risk / Unclassified), labeling compliance flag. If compliance is low, flag it —
   the data is unreliable and the reader needs to know.

5. **Operations** — ETRC scorecard, incident summary, LinearB velocity metrics.
   State the grade, not just the number. A C is a C.

6. **Risk Register** — RAID log content per team. Risks, assumptions, issues,
   dependencies, decisions. Raw is fine — the reader can parse it. What matters
   is that it's present and current.

**What the public version omits:**
- Suggested questions (those are 1:1 tools, not peer information)
- Personnel disclosures (medical, personal, family — anything that would be
  inappropriate in a broadly distributed document)
- Private coaching observations or corrective action context

---

## Template

```markdown
# SEM Report — [SEM NAME]
**Week Ending:** [DATE]
**Distribution:** [Public / Private]

---

## What Decisions Is Telling Me

### This Week's Update
[SEM card content verbatim, or: "No SEM card submitted for week ending [DATE]."]

### Goal Status
| Goal | Status | WoW Change |
|------|--------|------------|
| [Goal name] | [🟢 on-track / 🟡 at-risk / 🔴 off-track] | [delta or —] |

---

## Changes This Week

[Bullet list of week-over-week deltas: delivery date shifts, ETRC changes,
 velocity moves. If none: "No significant changes this week."]

---

## Delivery Health
| Team | Version | Planned Date | Projected Date | Status | Progress |
|------|---------|-------------|----------------|--------|----------|
| [Team (ENG##)] | [Version] | [Date] | [Date] | [🟢/🟡/🔴] | [X%] ([done]/[total] SP) |

> **Impacted Epics ([at-risk team]):** [Epic name] ([N] stories, [N] pts), ...
> [Omit this line if all teams are on-track.]

---

## Time Allocation ([Quarter])
**[TEAM]** ([Version]) — [N]h total
  [Work type breakdown: Feature: X% | Tech Debt: X% | Risk: X% | Unclassified: X%]
  - [Epic name]: [N]h ([X]% of capacity)
  [⚠ Labeling compliance: X% — work type classification may be unreliable]
  [Or: ✓ Labeling compliance: X%]

---

## Operations

### ETRC Scorecard
| Overall | Operations | Security | Finance |
|---------|-----------|----------|--------|
| [Grade] | [Grade (score)] | [Grade or N/A] | [Grade or N/A] |

**Operations Component Breakdown:**
| Indicator | Grade | Score |
|-----------|-------|-------|
| Major Days Breached | [Grade] | [Score] |
| MI Error Budget | [Grade] | [Score] |
| Minor Days Breached | [Grade] | [Score] |

### Incident Summary
| Team | Open P1 | Open P2 | MTTR (7d) | Health |
|------|---------|---------|-----------|--------|
| [Team] | [N] | [N] | [Xh or —] | [🟢/🟡/🔴] |

### Engineering Velocity (LinearB)
| Metric | Value |
|--------|-------|
| Cycle Time (p50) | [Xh] |
| PRs Merged | [N] |
| PRs Opened | [N] |
| Commits | [N] |

---

## Risk Register

### [Team Name]

**Risks:** ([N])
[RAID log content — paste raw from source. Do not summarize.]

**Assumptions:** [None / content]
**Issues:** [None / content]
**Dependencies:** [None / content]
**Decisions:** [None / content]
```

---

## Annotated Example — Temi, Week of May 11

The Temi report illustrates the pattern when a SEM card is missing:

```
## What Decisions Is Telling Me

### This Week's Update
No SEM card submitted for week ending 2026-05-11.

### Goal Status
[No goal status available due to missing card submission.]
```

The report doesn't infer or substitute. Missing is missing. The reader
knows the data gap immediately and can ask about it in the 1:1.

The Changes section shows the delta without narration:

```
## Changes This Week

- Delivery shift: ENG22 projected date moved 7 business days earlier (Jun 4 → May 26)
- Delivery shift: ENG46 projected date moved 19 business days earlier (Sep 1 → Aug 5)
- ETRC score change: Operations Total Score improved from A (3.60) → A (4.00), delta +0.40
```

Three facts. No interpretation. The reader brings the context.

---

## Voice Notes

**This document is not a narrative.** It is a structured data artifact. The
voice is in the selection and framing of what gets surfaced, not in prose
transitions between sections.

**Missing data is named, not hidden.** If the SEM didn't submit a card, say so.
If labeling compliance is 0%, flag it. The reader needs to know when the
underlying data is unreliable.

**The public version is not a sanitized version — it is a scoped version.**
The private version has more signal, not better signal. What's removed from
the public version is personnel context that would be inappropriate to
distribute broadly, not analytical content.

**Suggested questions are a 1:1 tool, not a peer communication.** They are
generated to prompt Joe's thinking before a direct report conversation. They
are not appropriate in a document distributed to peers — they imply a
supervisory relationship the peer audience doesn't have.

**The report travels as an artifact, not a message.** The Teams or email
message that distributes it is an `artifact_broadcast` — one sentence pointing
to the document. The document is the communication.
