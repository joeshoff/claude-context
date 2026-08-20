# Document Audit Prompt
_Run this on any draft before it goes up or out._

---

## The Prompt

Paste this into Claude with your draft appended below it:

---

**Audit this document against the following criteria. For each criterion, give a one-line verdict (pass / fix / missing) and, where the answer is fix or missing, quote the specific sentence or section that fails and rewrite it.**

**1. Does the document open with the conclusion?**
The first sentence or paragraph should deliver the bottom line: the diagnosis, the decision, the verdict, or the ask. If the reader has to get to paragraph two or three before they know what this is about, it fails. Throat-clearing, context-setting, and background sections at the top are failures.

**2. Is the supporting logic grouped correctly?**
Arguments should cluster by type: completed work together, live risks together, decisions needed together. If risks and wins are interleaved, or if action items are buried inside status paragraphs, the structure is broken.

**3. Are assumptions visible in the claim itself, not buried in caveats?**
Every projection, estimate, or forward-looking statement should carry its assumption inline. "This shows completion in late May" is naked. "This shows completion in late May, assuming 25% buffer and current velocity holds" is not. Find naked claims and flag them.

**4. Are there hedges where there should be decision rules?**
Flag any use of: may, could, might, potentially, seems to, appears to, it's possible that, we should consider. Each one should be replaced with either a clear causal statement ("if X, then Y") or an explicit acknowledgment of uncertainty with a named threshold ("I don't have enough data to call this until [condition]").

**5. Is ownership assigned or hidden?**
Passive constructions hide accountability. "It was decided," "work is being done," "this will be addressed". Flag all of them. Each action needs a named owner and a date or condition.

**6. Does the close match the document's purpose?**
- If no action is required: the document should end when the information ends. No "let me know your thoughts."
- If a decision is needed: the close should state what the decision is, what the options are, what the recommendation is, and when an answer is needed.
- If action is required: the close should name who does what by when.

**7. Scope check: what can be cut?**
Identify any section, paragraph, or sentence that does not advance the conclusion or support the decision. Background that the reader already has. Context that doesn't change the ask. History that isn't load-bearing. Flag it for removal.

---

**Output format:**
For each criterion: `[CRITERION #]: [PASS / FIX / MISSING]`
If fix or missing: quote the failing text, then rewrite it.
End with a one-paragraph overall verdict: what's structurally sound, what's broken, and the single highest-leverage fix.

---

## When to Use This

- Any upward communication to VP+ before it sends
- Exec one-pagers and proposals
- Escalations where the stakes are high enough to warrant a second pass
- Any document you've drafted quickly and aren't sure is landing right
- Anything you've been asked to review for someone else

## What This Doesn't Cover

This audit checks structure and argument logic, not voice, tone, or factual accuracy. Run it after you've drafted, before you send. If the content isn't right yet, fix the content first. This tool finds structural problems, not knowledge gaps.
