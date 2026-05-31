---
type: exec_one_pager
register: direct, compressed, owns the judgment
audience: VP and above, skip-level stakeholders, cross-org decision-makers
when_to_use: >
  A standalone document making a single argument to a senior audience. Use when
  the ask or proposal is too complex for a status update but doesn't warrant a
  full deck or memo. Covers: proposals requiring budget or headcount, requests
  for a decision that's stalled, org or process changes needing VP buy-in,
  risk escalations that need a named response. One argument per document.
  If you have two arguments, write two one-pagers.
---

## What Makes This Different From status_update_up

`status_update_up` is a recurring status artifact. It reports current state.

The exec one-pager makes an argument. It is a persuasion document with a
specific ask. The reader should finish it knowing: what is true, why it
matters, what you're recommending, and what you need from them.

The Pyramid Principle structure applies explicitly here:
- **Conclusion first** — the answer before the evidence
- **Grouped support** — evidence clustered by type, not by chronology
- **Visible assumptions** — no naked claims
- **Single ask** — one decision per document

---

## Structural Pattern

```
SUBJECT / TITLE: [The ask or the verdict — not a description of the topic]

PARAGRAPH 1 — THE POINT
One to three sentences. What is true right now and what you are recommending.
No wind-up. The reader knows the conclusion before they hit the evidence.

PARAGRAPH 2 — THE SITUATION (why this is in front of them now)
What created this moment. Not history — the specific condition that makes this
decision live. One constraint, one trigger, or one data point that explains
the timing. If the situation is obvious to the reader, compress or cut.

PARAGRAPH 3 — THE EVIDENCE (grouped by type)
Facts that support the conclusion. Risks, data, prior attempts, dependencies.
Grouped by type — not chronological. Assumptions embedded in the claim, not
footnoted. If there are competing options, name them here and dispose of the
weaker ones in one sentence each.

PARAGRAPH 4 — THE ASK
One ask. Decision, resource, authority, or presence. Decision-rule form:
"I am proceeding with X unless you redirect me by [date]" or
"I need [specific thing] by [date] to [specific outcome]."
Name the consequence of inaction if it is material.

[OPTIONAL — CONSTRAINTS OR PRIOR ATTEMPTS]
What you've already ruled out or tried, embedded as a constraint.
"I've already asked [X], who referred it back." Prevents the reader
from suggesting the thing you've already discarded.
```

---

## Template

**Subject / Title:** [What this is recommending or deciding — active voice, not topic label]

[THE POINT — conclusion stated plainly. What you are recommending and why in
one to three sentences. The reader knows the verdict before they read the evidence.]

[THE SITUATION — one to two sentences on what makes this decision live now.
The trigger, the constraint, or the timing. Cut if the reader already has this context.]

[THE EVIDENCE — two to five sentences, grouped. Data, risk, options considered
and disposed of. Assumptions embedded. "This assumes [X]" lives in the sentence,
not at the bottom of the document.]

[THE ASK — one sentence. Decision, resource, authority, or alignment.
If you're proceeding absent direction, say so and name the date.
If inaction has a named cost, name it.]

[OPTIONAL — constraints or prior attempts, one to two sentences.]

---

## Annotated Examples

### Example A — Headcount / Resourcing Ask

**Subject:** Request: Convert Two Contractor Roles to FTE Before Q3 Planning Lock

We should convert Ashwin Mehta and Dana Rowe from contract to FTE before
Q3 planning closes. Both are performing above the level they're billed at,
both are at retention risk, and the cost delta over a 12-month horizon
favors conversion — assuming standard WGU benefits load, the break-even
is month 4.

The Q3 headcount lock is June 14. After that, any conversion requires an
exception process through TA that adds 6–8 weeks. This is the last clean
window.

Ashwin is billed as a Sr. SE but performing at a level I'd rate SE II —
I'd convert at SE II, above average for that band. Dana is straight SE II,
no gap. Both have indicated informally they'd accept offers; I haven't
made a formal approach pending your direction. The third contractor on
the list (Fernando Reyes) is EDMO-sourced and I don't expect conversion
is possible — I've excluded him from this ask.

I need a yes or no by June 10. If yes, I'll initiate with TA immediately.
If no, I'll work the retention problem a different way — but I want you
to know the window closes.

---

### Example B — Process Change / Risk Escalation

**Subject:** JIRA Velocity Data Is Unreliable — Here's What I'm Using Instead and Why

The Jira projection numbers for ENG30 and ENG26 are not trustworthy right
now and I am not using them for delivery forecasting. I'm working from a
spreadsheet model with assumed velocity and weekly recalibration. Current
view shows ENG30 completing in late August against a September 7 target —
early, but the assumption load is high.

The specific problem: partial work isn't counted toward completion in the
version report, which means teams that are mid-sprint look later than they
are, and teams gaming story point closure look earlier than they are. I've
flagged this to the SEMs. It hasn't been fixed yet.

I'm raising this because I don't want you reading a green dashboard and
thinking the underlying picture matches it. The spreadsheet model is the
ground truth until Jira hygiene improves. I expect that to be resolved
by end of sprint 4 — Rebecca is running it down.

No ask here. Situational awareness only. If you want the spreadsheet
model in your weekly packet instead of the version report numbers, say
the word and I'll route it there.

---

## Voice Notes

**The title is the verdict, not the subject.**
"Request: Convert Two Contractors" tells the reader the ask before they
open the document. "Re: Contractor Conversion Discussion" does not.
The title should function like a subject line on a corrective action —
diagnostic, not descriptive.

**One ask per document.**
If you have two decisions that need to be made, write two one-pagers.
Bundling asks dilutes both and gives the reader an easy out: "Let me
think about the package." Separate asks force separate answers.

**Evidence is grouped, not chronological.**
Don't tell the story of how you got here. Group: data that supports the
conclusion, risks or constraints, options you've already disposed of.
Chronology is for the appendix.

**"I am proceeding unless you redirect me" is not aggression — it's service.**
Senior readers are busy. Giving them a default path with an opt-out is
easier than asking for active approval. Use it when you have enough
authority to own the outcome if they don't respond.

**Constraints belong in the body, not in a footnotes section.**
"This assumes standard benefits load" lives in the sentence where the
cost claim appears. Not at the bottom. Not in parentheses at the end.
Naked claims — projections without assumptions — are the most common
structural failure in upward communication.

**If there's no ask, say so explicitly.**
"No ask here. Situational awareness only." This prevents the reader
from searching for a decision they're not being asked to make, and
signals that you're not abdicating — you're informing.
