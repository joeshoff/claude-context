```markdown
---
type: management_inquiry
register: direct / low-ceremony
audience: direct reports (engineering managers, tech leads)
when_to_use: |
  You have a data point, a discrepancy, or an observed gap and need the
  direct report to account for it and name their plan. The diagnosis is
  already formed — the question carries it. Use when you want accountability
  without triggering defensiveness: you're asking what they're doing about it,
  not reciting what they did wrong. Works across async (Teams chat, email) and
  as a prep frame before a sync.
---

## Structural Pattern

1. **Name the data or list.** State what you're looking at — raw, no editorializing. This grounds the inquiry in fact, not impression.
2. **Expose the gap or unknown.** One sentence. Not an accusation — a visible discrepancy. "I don't know where these come from." / "It's gone from 2 weeks late to a month."
3. **Conditional decision rule.** IF [condition], THEN tell me [specific thing]. Not open-ended — the question has a shape.
4. **Precision filter.** Name what you're NOT asking for so the answer doesn't drift. Capability vs. capacity. Above average, not just present. A plan people believe, not a plan.
5. **Watch-outs (optional).** If there's a downstream action or a trap the person is likely to fall into, flag it explicitly. No softening.
6. **Raw data, inline.** Drop the list or artifact directly. No attachment theater.

Rhythm note: short declarative → exposed gap → conditional question → filter → data dump. The question does the disciplinary work so the declaration doesn't have to.

---

## Template

```
These are [WHAT YOU'RE LOOKING AT — e.g., "the contractors I have listed for you" / "the sprint metrics for [TEAM] as of [DATE]"]:

I don't know [WHAT'S MISSING OR UNCLEAR — e.g., "where they come from ([SOURCE HYPOTHESIS]? somewhere else?)" / "why this wasn't flagged before Monday"].

IF [CONDITION — e.g., "we can convert them" / "there's a plan to close this"], tell me [SPECIFIC DELIVERABLE — e.g., "WHICH ones you think would ADD to our capabilities (not just capacity)" / "what the actual sequencing looks like and who owns each piece"].

[PRECISION FILTER — name what you're not asking for:]
Not [EXCLUDED ANSWER — e.g., "just capacity adds" / "a restatement of the timeline"]. I expect [WHAT ABOVE-AVERAGE/CORRECT LOOKS LIKE — e.g., "[NAME] is billed as a Sr. SE but is performing at SE I — convert at that level or not at all" / "a risk in the registry and a plan the team will actually execute"].

[OPTIONAL — WATCH OUT FOR:]
[NAME THE TRAP OR DOWNSTREAM CONSEQUENCE — e.g., "Compressing [X] weeks into [Y] weeks left means [Z] days/week. That's [SPECIFIC IMPLICATION — weekends, nights, etc.]." / "If [PERSON] comes Monday without specifics, that meeting is a waste."]

[RAW DATA / LIST / ARTIFACT — pasted inline, no summarizing]
```

---

## Annotated Examples

### Example A — Contractor Conversion (Teams chat, condensed)

> These are the contractors I have listed for you: I don't know where they come from (IG? somewhere else?). IF we can convert them, tell me WHICH ones you think would ADD to our capabilities (not just capacity --> they are above average --> OR what level would you convert them at to make them above average i.e. BOB is billed as a Sr. SE but nope. As an SE I, he would be above average. (I recognize EDMO names in here for some reason e.g. Ashish Fernando ... so I imagine there's a fair number of them we won't/can't convert.)

**What's happening structurally:**
- "I don't know where they come from" = exposed gap, not a reprimand. The manager now has to explain provenance.
- "IF we can convert them" = Joe isn't assuming they're convertible. The conditional protects against a useless answer.
- "not just capacity" = precision filter. The exclusion is doing as much work as the question.
- The BOB example = a concrete decision rule embedded in the question. It tells the manager exactly what calibration Joe expects before they answer.
- The EDMO aside = Joe names his own assumption out loud so the manager doesn't waste time on names Joe already expects to be off the table.

---

### Example B — Sprint Gap Escalation (Teams chat)

> Here is the beauty of having data. Version report shows Eng 25 2 weeks late as of Monday. Blake tries to tell me it is the version report and he is confident. Version report lies, because partial work isn't counted (exactly the point I say). But his sprint ended yesterday, so let's go look. It's gone from 2 weeks late to a month. I was having the old Jedi mind trick played on me — with the data in front of our faces, it didn't work. Compressing 4 weeks with 2 weeks left is 2.5d/week everyone must work. That is Saturday Sunday and extra nights. WATCH OUT FOR: I told him he had a) better get a risk in his registry about this b) must come Monday with an actual plan that people believe will close that now very large gap. Please let me know how that goes.

**What's happening structurally:**
- "Here is the beauty of having data" = leads with the diagnostic frame, not the charge. The data speaks; Joe annotates.
- "Version report lies, because partial work isn't counted" = names what's broken, assigns no blame to the person — just corrects the bad instrument the person was relying on.
- The math ("2.5d/week") = Joe compresses the consequence into a single arithmetic statement. No hand-wringing about what it "might mean for the team."
- "WATCH OUT FOR" = explicit trap flag passed upstream to the skip-level manager. Joe isn't softening it — he's telling them what to watch for in the Monday meeting.
- "a plan that people believe will close that now very large gap" = the precision filter. Not a plan. A plan that is believed. The bar is named.

---

## Voice Notes

**What makes this type distinctive in Joe's register:**

1. **The question carries the verdict.** Joe never says "you did this wrong." He asks "IF we can convert them, which ones ADD to capability?" — which already implies some of them don't, and the manager should know that. The inquiry does the accountability work.

2. **Conditionals over declarations.** "IF we can convert" / "IF there's a real plan" — Joe doesn't assume the answer. But the conditional structure means the manager can't dodge with a yes/no.

3. **The exclusion is mandatory.** Every inquiry names what he's NOT asking for. "Not just capacity." "Not a restatement." The precision filter closes the escape routes without closing the question.

4. **Data inline, no attachment theater.** The list goes in the message. This is a power move — it eliminates "I didn't see the attachment" and forces the conversation to happen on top of the raw evidence.

5. **Caps for emphasis, not decoration.** WHICH, IF, WATCH OUT FOR — these are navigational, not emotional. They tell the reader where the answer is expected to land.

6. **Assumptions owned and named.** "I imagine most are iSC so probably not a big list." Joe doesn't pretend he has no prior. He states his assumption so the manager can confirm or correct it — not rediscover it.

7. **Watch-outs pass the load up or across.** When a consequence is serious, Joe doesn't embed it gently. He names it ("Saturday Sunday and extra nights") and flags it for whoever needs to hold the person accountable next.
```