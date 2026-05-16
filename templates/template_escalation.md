```markdown
---
type: escalation
register: direct-urgent
audience: peer-level leaders, skip-level managers, cross-functional decision-makers
when_to_use: >
  Diagnosis is complete and you need a decision, resource, or blocker removed — not a discussion.
  Use when the problem has already stalled at your level, when ownership is unclear and no one is
  moving, or when the cost of inaction now exceeds the cost of the conversation. Not for venting.
  Not for FYI. The reader must be able to act on this message alone.
---

## Structural Pattern

```
0. BLUF — one sentence orienting the reader to what this is about and what you need.
   Calibrate to audience:
   - Upward (to Hank alone): verdict + ask. "X is broken and I need a decision."
   - Peer + up (to peers CC'd to Hank): frame + coordination ask. "We need to do Y together."
   The BLUF is not the full argument. It's the reason to keep reading.

1. STATE WHAT'S BROKEN (one sentence, present tense, no hedge)
2. NAME THE STALL (who or what is blocking resolution — be precise)
3. COST OF INACTION (concrete: student impact, team capacity, deadline, legal/policy exposure)
4. YOUR SPECIFIC ASK (decision, resource, authority, or presence — one ask per escalation)
5. [OPTIONAL] CONSTRAINT OR ASSUMPTION EMBEDDED IN THE ASK
```

The skeleton is tight by design. If diagnosis requires more than 3 sentences, the problem isn't
ready to escalate — it needs another round of triage first. No background sections. No history
lessons unless they explain why this is stuck *right now*.

**On humor in serious-but-not-furious escalations:** A dry observation or sardonic aside is
appropriate when the register is "I need us to fix this" rather than "I am done." It signals
confidence, not anger — you can afford the wit because you're not at the breaking point yet.
One line, placed after the diagnosis lands, before the ask. If you're genuinely pissed, skip it.

---

## Template

**Subject:** [System/Process/Person]: [What's broken, not what happened]

[BLUF — one sentence. Upward: "X is broken and I need [decision/action]." Peer+up: "We need
to [coordinate / align / move together] on [topic], quickly." Not the full argument — the frame.]

[WHAT'S BROKEN — one sentence. Name the thing. Not "there have been concerns about" —
"[X] is not [doing / working / deciding] and [Y] is the result."]

[OPTIONAL: One dry observation if the register is serious-but-not-furious. Skip if pissed.]

[THE STALL — who owns it on paper, why it hasn't moved, what's been tried.
If ownership is genuinely unclear, say that directly: "No one has claimed this."]

[COST — what happens if this stays unresolved past [DATE/MILESTONE].
If the cost is to a student, name it. If it's to the team, name it. Don't generalize.]

[THE ASK — "I need [decision / approval / your presence / ownership assigned] by [DATE].
If [condition], then [path forward]. If not, [what Joe will do or stop doing].]

[OPTIONAL: What Joe has already ruled out or tried, embedded as a constraint —
"I've already asked [X], who referred it back. That loop needs to stop here."]

---

## Annotated Examples

### Example A — Ownership gap on a stuck student ticket (Teams chat)

> Blake Wilcox — please look at this. [SERVICENOW LINK] You were on the escalation thread.
> I do not know what is going on or why it is necessary for SD to escalate this up to tier 3,
> but this poor student has been stuck forever.
> 1) Who owns it — instead of batting it around it'd be great if someone would just run it down
>    until it was resolved
> 2) Where is that hard-coding that Daniel Crosby refers to? If he is correct, that would clearly
>    identify ownership. Somebody owns that. And if it is Enrollment/SSE then this is an edge case
>    it seems our SD and AppSupport teams are not equipped to handle, correct?

**What's broken:** Ticket has been passed around without resolution. A student is blocked.
**The stall:** No one has taken ownership. Teams are batting it laterally.
**Cost:** Student harm — named ("this poor student has been stuck forever").
**The ask:** Two direct questions that, answered, produce ownership. Not "let's get together."
**Constraint embedded:** If Daniel Crosby is right, ownership is traceable. Joe's not asking
for a debate — he's asking someone to verify a claim and act on it.

**Voice note:** No greeting, no sign-off, no "I wanted to flag this." The link comes first.
The numbered list isn't organizational courtesy — it's two specific assignments handed to Blake.

---

### Example B — Performance/HR process blocked by org friction (email)

> Subject: FW: Response to FWW to Raj Singh
>
> What message should I be learning from all of this exactly? My inclination: Do NOT under any
> circumstances put people on corrective actions. We WILL continue to give them the rating we
> think it deserves, but at this point — since there seems to be little appetite to fix this
> problem with P&T/Employee Relations — all we can do is hope that underperformers eventually
> get the message.
>
> This is exactly the scenario I feared in January, when I said in my presentation "Cultural
> change is crucial... If we don't fix things here nothing else we say or do will matter."
>
> I am laying down my weapons of war since this seems to be a problem we just can't fix.

**What's broken:** HR/P&T will not back corrective actions. The performance accountability
process is functionally inoperable.
**The stall:** P&T and Employee Relations are not engaging. The loop is closed against the
manager doing the work.
**Cost:** Named explicitly — culture rot. The January prediction is now an "I told you so"
with receipts, not a grievance.
**The ask:** Implied but sharp — *either fix this or tell me to stop trying.* "Laying down
my weapons" is not resignation; it's a final move forcing a decision from above.
**Constraint embedded:** "Since there seems to be little appetite to fix this" — Joe has
already surfaced this before. This isn't the first notice.

**Voice note:** The rhetorical question at the top ("What message should I be learning?") is
not genuinely open. It's a forced choice handed upward. The quote from the January presentation
embeds the proof that this was predicted and ignored. No labeled sections. No bullet points.
The escalation is structured as argument, not report.

---

## Voice Notes

**What makes Joe's escalations distinct:**

1. **Diagnosis precedes the send.** He doesn't escalate to think out loud. By the time it
   goes up, he knows what's broken and why. The message is the conclusion, not the discovery.

2. **The ask is binary or specific.** "Who owns this?" "Do I need to be in the room?"
   "Should I stop trying?" He doesn't ask for advice. He asks for a decision or an action.

3. **Frustration is data, not complaint.** "I am laying down my weapons of war" is a signal,
   not a tantrum. It tells the reader: this has reached a breaking point and I need you to
   decide whether to intervene or give me permission to stop.

4. **He names the person, not the role.** Blake Wilcox, Daniel Crosby, Peter Russell — not
   "the service desk team" or "HR." Accountability is personal.

5. **Embedded constraints compress the ask.** He doesn't write a paragraph of context and
   then ask a question. The context *is* the question. "If Daniel Crosby is correct, that
   would clearly identify ownership" — the condition and the conclusion are in the same
   sentence.

6. **No throat-clearing, no sign-off niceties on hot escalations.** The Teams chat examples
   open with a name and a link. The email examples open with the blunt observation.
   Closing pleasantries disappear when the stakes are real.
```