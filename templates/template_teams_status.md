```markdown
---
type: teams_status
register: internal
audience: engineering leadership, SEMs, direct reports
when_to_use: >
  Recurring or ad-hoc status drops in a Teams channel. Use when you need to
  establish the verdict on one or more teams/workstreams at a glance, then
  supply the evidence and the mechanism (what's actually causing the state).
  Emoji signal is appropriate when the channel already uses them; omit if the
  channel is purely text-formal.
---

## Structural Pattern

```
[SIGNAL EMOJI] [VERDICT LABEL] (optional: "ongoing" / "as of [date]")

[TEAM NAME] ([LEAD]) — [one-sentence delivery verdict + date/variance].
[Completion metric: X% complete (n/N SP).]
[RAID or signal layer: what the surface metric hides.]
[Named risk or mechanism: the actual thing driving the state.]
[Judgment sentence: what this means, no hedge.]

[Repeat block per team.]

[Optional closer: the one or two things that need to surface to a named stakeholder, and why.]
```

**Signal emojis (use when channel culture supports):**
- 🟢 ON TRACK
- ⚠️ AT RISK
- 🔴 OFF TRACK
- ➡️ NEUTRAL / MONITORING

**Rules:**
- Verdict first, always. Evidence is the second sentence. Mechanism is the third.
- If surface metrics (Jira) contradict RAID, say so explicitly. Name which to trust.
- Do not average across teams. Each team gets its own verdict.
- If a risk has no owner or no resolution path, name that gap directly.
- The closer (if present) names the exact person who needs to act and why now.

---

## Template

```
[🟢/⚠️/🔴/➡️] [VERDICT LABEL] [(ongoing) if applicable]

[TEAM NAME] ([LEAD]) — projecting [DATE], [Nd early/late]. [X]% complete ([n]/[N] SP). [One sentence: what the RAID or signal layer reveals that the Jira number doesn't.] [Named mechanism: the specific risk, blocker, or dependency driving the state — include owner or note if unowned.] [Judgment: what this actually means for delivery, one sentence, no hedge.]

[TEAM NAME] ([LEAD]) — projecting [DATE], [Nd early/late]. [X]% complete ([n]/[N] SP). [RAID/signal layer sentence.] [Named mechanism.] [Judgment sentence.]

[Repeat as needed.]

[OPTIONAL CLOSER — use when something needs to escalate:]
The [one/two] things I'd put in front of [NAME]: [ISSUE A] and [ISSUE B]. [One sentence on why — what changed, what's missing, what the urgency is.]
```

---

## Annotated Examples

### Example A — Multi-team, mixed verdict

> 🟢 ON TRACK
>
> ENG29 Intake 2 (Blake) — projecting May 30, 31d early. 54.2% complete (150/277 SP). But the RAID log is the most active in the org — 10 risks and 38 dependencies, several marked Active/Critical: EDMO security compliance (FERPA, subprocessor agreements, LLM disclosures) are called out as "formal delivery blockers for production access." Mexico Summit + PTO impacted the week of May 4. Blake is managing a lot of open risk for a team that looks fine in Jira.
>
> ENG22 Partnerships (Temi) — projecting Jun 4, 26d early. 71.8% complete (102/142 SP). Still delivering despite the RAID showing severe attrition: 3 of 4 Salesforce engineers gone, Solutions Architect (Mariyam) moved to another team, Hugo departed. The RAID lists this as "mitigating" but there's no resolved path. Heroic delivery on a fragile foundation.

**What's working:**
- "Looks fine in Jira" / "fragile foundation" — the judgment sentence lands the real state in one phrase, no elaboration needed.
- RAID evidence is specific: named blockers, named people, named status codes. Not "some risks exist."
- 🟢 applies to the label, not the full picture. The body corrects the emoji for the reader. That tension is intentional.

---

### Example B — At-risk, with closer

> ⚠️ AT RISK (ongoing)
>
> ENG30 Triforce (Rebecca) — actually improved. Was Sep 7 (69d late), now Aug 17 (48d late). Still deeply at risk at 18.6% complete (58/311 SP), but moving in the right direction. RAID confirms the two blockers: Kafka bugs in testing, and Salesforce engineering shortage flagged explicitly by Rebecca. The SF resource risk has no owner resolution on it.
>
> ENG26 Edgerunners (Rebecca) — projecting Jul 8, 8d late. 31.4% complete (61/194 SP). RAID is concerning here — logged risks include "no stories yet, just high-level requirements" on at least one piece of work, a "major risk" around a program launch date with no commitment made yet, and several open scope questions. The RAID suggests there's more at-risk than the 8-day Jira variance implies.

**What's working:**
- "No owner resolution on it" — this is the mechanism sentence doing its job. It names the gap, not the worry about the gap.
- Week-over-week comparison ("Was Sep 7... now Aug 17") establishes trajectory without a chart.
- Closer format (from Example 5 in the source set): "The two things I'd put in front of Hank: the Intake 1 freefall and Delta's sudden reversal. Both changed dramatically in one week and neither has a RAID explanation attached." — Names the person, names the issues, explains why now (one-week change, no RAID cover).

---

## Voice Notes

**What makes this type distinctive in Joe's register:**

1. **The emoji is a claim, not a decoration.** 🟢 does not mean "everything is fine." It means "the Jira projection is green." The body of the update is where the real verdict lives. Joe uses the tension between emoji and text deliberately.

2. **RAID vs. Jira is the recurring diagnostic frame.** Surface metric (Jira velocity, projected date) is always checked against the RAID. If they diverge, name the divergence. "Looks fine in Jira" is a warning phrase, not a compliment.

3. **Judgment sentences are declarative, not speculative.** "Heroic delivery on a fragile foundation." "The SF resource risk has no owner resolution on it." These are conclusions, not observations. Joe does not write "this may indicate a concern" — he writes what the thing is.

4. **Named people, named risks.** Anonymizing or abstracting risks ("some resource constraints exist") is not this register. If Mariyam moved, say Mariyam moved. If there's no owner, say there's no owner.

5. **The closer escalates to a named person with a reason.** Not "FYI" — "the two things I'd put in front of [NAME]" with an explanation of why those two and why now. The closer is optional; use it only when something actually needs to move.

6. **Week-over-week trajectory is evidence, not context.** "Was 21d late last week, now projecting 13d early" is a data point that changes the verdict. Include it when the trend is the story.
```