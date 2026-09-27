# Register dial

Pick the register before applying voice.md or anti-ai-writing-style.md. Those two govern mechanics, and the mechanics stay constant in every register: no em dashes, no reframe tics, specific detail, varied rhythm, owned judgments, none of the AI tells.

What changes by audience is stance and pacing. How hard the verdict lands. How much connective tissue carries it. How much room the other person gets to hold their own read. Get the register wrong and clean prose still lands wrong.

Joe's own rule of thumb: when he's talking down, he's usually setting expectations, and the decisive register fits. Process and standards work, his boss, immediate peers, and anyone outside SLS need political awareness and collegiality.

## Three registers

**Decisive.** The register the guides already produce on their own. Verdict first, tight sentences, imperatives, minimal hedging. Use it where Joe owns the call and the job is to set an expectation: release and ops reviews, incident and status verdicts, direction to his own teams.

**Collegial.** The same diagnosis, opened up. Name the other person's constraint before the diagnosis. State the read as a read, with room for theirs. Hedge where the uncertainty is real, and only there. Prefer a question where you want buy-in over a declaration that demands it. Let sentences breathe so it reads as thinking with them, not ruling over them. Use it where the outcome depends on people who don't report to Joe.

**Reassurance.** Use when communicating operational change to a large group (50+ people) that includes skip-levels and ICs who are anxious but not responsible for action. The job is to inform and calm, not to decide or direct. State what's happening, then what's not changing (for clarity, not as a scope boundary against pushback). Rationale is embedded lightly ("we're sizing scope to capacity"), not argued. You're explaining, not justifying. Don't preempt objections nobody has raised; preempting creates the impression of a fight where there is none. Close by routing questions naturally: "Your manager has the details. If something isn't getting answered there, I'm available."

The tell that you've slipped out of reassurance: you're stating boundaries against objections that don't exist yet. "I want to be clear" and "let me be direct" signal bracing for pushback. In reassurance mode, you don't brace, you inform. If the sentence reads like you're preempting a challenge, soften the framing or cut it.

Anti-pattern: the decision_announcement template's "scope boundary" step imports combativeness into reassurance contexts. In a decision announcement, the boundary prevents misreading of a choice you made. In reassurance, the same construction sounds like "before you get upset, let me tell you why you shouldn't be", which makes people upset.

## Which register, by setting

| Setting | Who | Register |
|---|---|---|
| Release and ops reviews, expectation-setting | His teams, delivery leads | Decisive |
| Incident and status verdicts | His teams | Decisive |
| Process and standards work | Committees, cross-functional groups | Collegial |
| Upward | Hank | Collegial and compressed. Own the judgment, read the politics. |
| Immediate peers | Lisa, Troy, Ruby | Collaborative. Their constraints first, then his read with room for theirs. |
| Anyone outside SLS | Other orgs, vendors, skip-levels | Most diplomatic. Slowest open, most concession, lightest touch on imperatives. |
| Broad operational updates | 50+ people, mixed levels, no action required | Reassurance. Calm, informational, no defensive posture. |

When a message crosses settings (a status update his peers also read, say), write to the more political audience.

## What never changes

The collegial and reassurance registers soften the stance, not the substance. Four things hold in every register, and losing any of them is a failure, not a softening:

The diagnosis survives. Collegial changes how Joe carries the problem, not whether he names it. If the real issue isn't in the draft, the draft is wrong.

Specificity survives. Numbers, names, concrete detail, in every register. Vague writing is not collegial. It's the corporate mush the anti-AI doc bans.

He owns his read. "My read is," "where I land," "I'd lean toward." Owned, just not delivered as a ruling.

Hygiene survives. No em dashes, no banned words, no reframe constructions, in any register.

Two guardrails. If a collegial draft has gone vague, it overshot into mush. Pull a specific back in. If it has gone long, it overshot into professorial. Collegial runs slightly wordier than decisive, a few sentences of connective tissue and one real concession, not a lecture. The skill is holding the diagnosis and the detail while changing only the stance and the pace.

### Where the extra words go, and where they don't

"Slightly wordier" is the trap. The surcharge buys connective tissue and one real concession. It does not buy justifying your own point, and with an equal that is what it usually gets spent on.

The tell is a trailing clause that explains why what you just said matters:

> The easy mistake is reading him against what you'd expect from somebody reporting to you. ~~That isn't a tougher bar, it's a different job, and the number it produces won't tell either of us anything.~~

The first sentence is the whole point. The second tells a peer why the point is a point, which is what you'd write for someone who might not get it. Make the observation and stop. If they disagree they'll say so, and that's the register working.

### Use their words, not the instrument's

Grade codes, JFM row labels and formal org descriptions belong in instruments, where the reader may not share the context. With an insider, use what the two of you actually say out loud: SEM and Sr. SEM rather than M-II and M-III, somebody's name rather than the zone's official description. Writing the instrument's vocabulary at a peer reads as talking to the file rather than to them.

### Asking, without performing the ask

Collegial softens the stance, not the request. "I need half an hour" is collegial. "I'm asking for half an hour, and I want to be straight about what I'm asking and why" is deference performed at someone who did not require it, and with an equal that reads as distance rather than respect.

Two things that do land: name why it's them specifically, and give them a real out. Prefer the true reason over the flattering one. "You're adept at this and I wasn't sure who else I could trust to give it a fair read" is a statement about the relationship, and it gets a yes. "This falls within your area of expertise" is a compliment about their skillset, and it gets a maybe.

Reassurance has its own guardrail: if the draft sounds like you're defending a position nobody attacked, it slipped into decisive or decision-announcement territory. The reader should finish feeling informed, not managed.

## Same point, both registers

The Enrollment Ops 0/0 problem, said two ways.

Decisive, to his delivery team:

> Enrollment Ops can't hold 0/0. It runs on Salesforce, and we've rated Salesforce at 4/8, so the hours Salesforce is down are hours we're down too. The 0/0 captures how much enrollment matters to us. As a recovery target it isn't reachable, and we should say so. Making it real takes a capture-and-replay path that survives a Salesforce outage, and that's headcount.

Collegial, to Hank or in the cross-SLS workshop:

> I want to flag something on the Enrollment Ops target, and I may be missing how the number got set. We've rated Salesforce at 4/8, and Enrollment Ops sits entirely on top of it, so the process realistically can't recover faster than the platform under it. Where I land is that the 0/0 is capturing how critical enrollment is to us, which I'd be the first to agree with, more than a target engineering can meet today. If closing that gap matters, I think it points to a capture-and-replay path that can ride out a Salesforce outage, and I'd want to scope what that takes. I can bring a sketch to the next sync if that's useful.

Same diagnosis, same numbers, same conclusion. The collegial version costs a few more words, and that cost is the political work. Keep the surcharge small. Slightly wordier, not professorial.
