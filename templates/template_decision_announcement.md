```markdown
---
type: decision_announcement
register: direct / low-ceremony
audience: direct reports, peer leaders, skip-level stakeholders
when_to_use: >
  A decision has been made and needs to be communicated. No vote pending.
  No consensus being sought. Use when the decision is yours to make, you've
  made it, and people need to know what changes and why. Works for org changes,
  process changes, role adjustments, new standing meetings, delegated missions.
  Scales down to a Teams message for low-stakes decisions; scales up to email
  for decisions with org-wide visibility or role implications.
---

## Structural Pattern

1. **State the decision immediately.** First sentence, no wind-up. What is
   happening, what has changed, or what has been assigned.
2. **Name the scope boundary.** What this decision does *not* affect. Prevents
   misreading and kills rumors before they start.
3. **Give the rationale in one move.** Why you made it. Not a defense — a
   brief, honest account. If the reason is partially selfish or pragmatic, say
   so.
4. **Surface the observable change.** What people will notice or need to act on
   because of this decision. Concrete, not abstract.
5. **Set the path forward.** Who does what, by when, in what sequence. If
   nothing is required of the reader, say so explicitly.
6. **Close on access, not invitation.** State how questions reach you. Do not
   ask for opinions on the decision itself.

---

## Email Template

**Subject:** [Short noun phrase naming the decision — not a question, not a teaser]

[Decision stated plainly. One or two sentences. What is now true that wasn't before.]

This is not [what this decision is NOT — scope boundary]. [Explain what stays
the same, if that needs saying.]

I [made / asked / assigned] this because [honest rationale — efficiency, risk,
gap in coverage, external deadline]. [If there's a tradeoff or imperfection,
name it briefly.]

You [will / may] notice [specific observable change — new behavior, new
touchpoint, new artifact, shifted responsibility]. [One sentence on why that's
fine or what to do if it's not.]

[WHO] will [WHAT ACTION] by [WHEN / in what sequence]. [If there's a
dependency or handoff, name it.] I [will / won't] be looped in at [specific
point].

If you have questions, [reach me directly / bring them to [FORUM] / send them
to [PERSON]].

---

## Teams Announcement Template

[Name or group] — [Decision in one sentence. What is now happening or assigned.]

[Scope boundary: what this does not change, if it needs saying.]

[Rationale in one clause or sentence.] [Deadline or external constraint if
one exists.]

[What the recipient needs to do, in sequence, with timeline.] [If nothing is
required: "No action needed from you."]

[How they reach you with questions.]

---

## Annotated Examples

### Example A — Role/Scope Adjustment (email)
*(Based on Example 3: Solution Architecture adjustment)*

> **Subject:** Solution Architecture (slight) adjustment
>
> I've asked Raj to help me out in specific areas to reduce coordination load
> on me and the SEMs.
>
> This is not a change to how SAs relate to teams, and no one's responsibilities
> shift except Raj's.
>
> I'm announcing it here because you may notice him asking about things outside
> his previous area. That's expected and intentional — not scope creep.
>
> Nothing required from you. If it raises questions, come to me directly.

**Why it works:**
- Decision is in sentence one.
- Sentence two does the scope-limiting work before anyone can misread it.
- The rationale ("reduce coordination load") is honest and self-aware — Joe
  includes himself as a beneficiary, which reads as credible rather than
  political.
- "Nothing required from you" is an explicit close — readers don't have to
  guess whether they have a task.

---

### Example B — Delegated Mission (Teams)
*(Based on Example 4: tech debt prioritization)*

> Raj — I need a prioritized technical debt list across the SLS portfolio,
> delivered to Lisa Moore by EoD March 18th.
>
> Work with the other SAs and SEMs to build it. The list needs: (a) brief
> description of the debt, (b) what it's costing us by not fixing it
> (MIs, man-hours, dollars), (c) rough effort to remediate (SPs, quarters,
> man-months — rough is fine) and what remediation looks like.
>
> I'll screenshot this and send it to the SEMs so they know it's coming.
> Include me as Optional on any meetings you schedule for this.

**Why it works:**
- No preamble. Mission is stated in sentence one.
- The deadline is named with its source ("Lisa Moore by EoD March 18th") —
  embedding the constraint gives the deadline authority without Joe needing
  to explain it further.
- The deliverable spec is a numbered list with enough detail to start work
  without a follow-up question.
- Joe's own role ("Include me as Optional") is explicit, preventing
  over-inclusion or under-inclusion.

---

## Voice Notes

**What makes this type distinctive in Joe's register:**

- **Self-inclusion in rationale.** Joe names when a decision benefits him
  ("mostly mine, but SEMs as well"). This isn't hedging — it's the opposite.
  It signals the rationale is real, not dressed up.

- **Scope boundaries are load-bearing.** "This is not a change in relationship
  of SA to teams" does more work than the affirmative statement. In Joe's
  templates, the boundary usually appears in sentence two or three, before
  any reasoning. Don't skip it.

- **Sequence is explicit when it matters.** In multi-step announcements, Joe
  names the order: *first* this, *then* that, *then* the broader group. He
  doesn't leave the reader to infer sequence from context.

- **Low ceremony, high specificity.** The register is conversational ("prob
  better coming from me," "ya'll") but the operational content is precise
  (exact deliverable fields, exact deadline, exact sequencing). Ceremony and
  specificity are inversely correlated here — the more casual the tone, the
  more exact the task definition needs to be.

- **The close names the decision's finality without being combative.** Joe
  doesn't invite debate on the decision, but he also doesn't say "this is
  final, period." He routes questions to himself or a forum — which implicitly
  says: *questions are fine, reversal is not on the table.*

- **Never use labeled sections in email form.** No bolded headers like
  "Rationale:" or "Next Steps:". The structure lives in the prose order, not
  in formatting scaffolding.
```