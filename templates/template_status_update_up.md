```markdown
---
type: status_update_up
register: direct, compressed, owns the judgment
audience: VP and above
when_to_use: >
  Weekly or ad-hoc status update sent upward. Use when the recipient needs
  current state, risk posture, and any decision required — without having to
  extract it from narrative. Works for email or as a forwarded summary thread.
---

## Structural Pattern

```
SUBJECT: [Team/Initiative] — [Week of DATE] or [specific trigger]

SENTENCE 1: The headline. One sentence. What is true right now.
  - If things are on track: say so and close that topic.
  - If things are off track: name the failure mode immediately.

BODY: Facts in order of consequence. Each fact either:
  (a) closes a loop ("X is done / shipped / resolved"),
  (b) names a live risk with a decision rule attached, or
  (c) surfaces a decision that is blocked at the recipient's level.

No transitional scaffolding. No topic sentences restating the subject line.
No "as mentioned" / "as you know" / "following up on."

If forwarding someone else's update: one-line framing ("Listed as highlight
this week" / "Flagging this — see risk in third bullet") then the chain.
If the body exceeds ~150 words, trim findings, not conclusions.

CLOSE: Either nothing (if no action needed) or a single crisp ask.
  - "I need a decision on X by [date]."
  - "I'm proceeding with Y unless you redirect me."
  Never an open-ended invitation.
```

---

## Template

**Subject:** [Team / Initiative / Domain] — [Week of DATE | ad-hoc: one-phrase trigger]

[One-sentence state of the world. No hedge. If good: "We're on track for [milestone] with one caveat below." If bad: "We have a slip on [thing] — details below."]

[COMPLETED / RESOLVED — list only what materially closes a loop:]
[Item 1: what finished, why it matters in one clause — e.g., "All 23 critical-through-low audit findings cleared and deployed in sse-common."]
[Item 2 if needed.]

[RISKS / PROBLEMS — list only what is live and consequential:]
[Risk 1: name the condition, the trajectory if unaddressed, and the mitigation in force or the mitigation gap — e.g., "JIRA projections aren't reliable yet; we're working from a spreadsheet with assumed velocity. Current view shows [date] against [target date]. Mitigation: [action owner] by [date]."]
[Risk 2 if needed.]

[DECISION NEEDED — only if blocked at recipient level:]
[What the decision is, what the options are, what I'm recommending, and when I need an answer. If I'm proceeding absent direction, say so: "I'm moving forward with [X] unless you redirect me before [date]."]

---

## Annotated Examples

### Example A — Forwarding a team win as a highlight

> **Subject: FW: Code Quality Audit Remediation Complete (sse-common)**
>
> FYI — listed as highlight for this week.

**What Joe did:**
- Subject line preserves the original finding so the VP can triage on read.
- Four words of framing ("FYI — listed as highlight this week") are the entire editorial layer. The implication: *this is good news, it's attributed, it's in the record.*
- No summary of the summary. No praise. The chain carries the detail.
- Works because the recipient can stop at the four-word line or drill into the PR table. Joe doesn't force them to read both.

**Pattern extracted:**
```
[One-line frame: why you're surfacing this — win / risk / FYI]
[Forward the chain. Nothing else.]
```

---

### Example B — Risk update with mitigation trajectory and open loop

> **Subject: Fw: Welcome+ Build Release review**
>
> Let me know if you have any questions/concerns
>
> [forwarded chain with dashboard links and key takeaways]
>
> **SST:** JIRA isn't quite working for projections yet, but SEMs are looking into it. Meanwhile, we work from a spreadsheet, with assumed velocity and 700+ points in the backlog. This shows completion in late May, early June against July 11 expectation but is the MESA team only. This view also assumes a 25% buffer and high uncertainty.
>
> Problems around CE and SF resourcing, some uncertainty about hand-offs leading to a backlog of completed work not making into production are problems we are working through.
>
> Architects are to a) talk to leads to hit the major pain points soonest and b) by end of next week have formal documentation to address. SEMs will work with their teams to ensure that they are fully engaged in solving these problems.

**What Joe did:**
- "Let me know if you have any questions/concerns" is the only wrapper — minimal, not warm. It signals *I'm accountable for what's below* without restating it.
- Each risk bullet names the condition first ("JIRA isn't quite working"), then the current trajectory ("late May, early June against July 11"), then the assumption baked into that estimate ("25% buffer, high uncertainty"). The VP gets all three layers in one read.
- Mitigation has owners and deadlines: "Architects are to a) ... by end of next week." No vague "we're addressing it."
- No closing ask because the decision isn't blocked — Joe owns the mitigation path.

**Pattern extracted:**
```
[Minimal framing — one line or nothing]
[Risk: condition → trajectory → assumptions]
[Mitigation: owner + deadline, or name the gap if there's no owner yet]
[Ask only if a decision is blocked upstream]
```

---

## Voice Notes

**What makes status_update_up distinctive in Joe's register:**

1. **The headline does the work.** Joe doesn't warm up to the point. If the audit is done, sentence one says the audit is done. If the schedule is slipping, sentence one says it's slipping. The reader never has to hunt.

2. **Forwarding is a communication act, not a pass-through.** When Joe forwards, he frames in one line. That line tells the VP how to feel about what follows before they read it. "FYI — listed as highlight" means *no action, just awareness*. A different frame — "Flagging a risk here" — would mean *stay alert*. The frame is the message; the chain is the evidence.

3. **Risk statements carry their own assumptions.** Joe doesn't say "there may be delays." He says "this shows completion in late May against July 11, assuming 25% buffer and high uncertainty." The VP can disagree with the assumption, but can't wonder what the assumption is.

4. **Mitigation has owners or it's named as a gap.** "We're working on it" never appears without an owner and a date, or an explicit flag that an owner is missing. If the mitigation is incomplete, Joe says so — "these problems either have mitigation plans or are working toward them" — not because it's reassuring, but because it's accurate.

5. **Cultural / structural context gets named plainly.** In Example 4, Joe doesn't soften "the processes aren't built yet" into "we're on a journey." He says: "Short answer: No, they are not completely built out." Then he explains why — not to excuse it, but because the VP needs to understand the constraint to make a good decision.

6. **No closing ritual.** Joe ends when the information ends. If there's a decision needed, he states it and names the deadline. If not, he stops. "Let me know your thoughts" does not appear.
```