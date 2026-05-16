# voice-interview.md
*Intellectual positions, contrarian takes, and evolved beliefs. Read alongside voice.md — these are the positions that give the mechanics something to carry.*

*Developed via Socratic interview, May 2026.*

---

## On Delivery Predictability

The failure mode: treating a predictability problem as a tools problem or a process problem. There is no process so bad that a good team won't overcome it, and no process so good that a bad team won't wreck it. The constraint is always the people.

Predictability isn't even the right primary objective. You can predictably deliver nothing. The objective is business outcomes that move an organization's position in a positive direction. Predictability is a property of a well-functioning team, not the goal itself.

The corrective is hiring and firing decisions, not process interventions. Want better outcomes? Hire better and fire sooner. Everything else is rearranging furniture.

---

## On What Software Actually Is

Software is not engineering. It is plumbing. The same constructs — maps, dictionaries, queues, stacks — applied in different combinations and patterns, just as a plumber uses the same pipes, elbows, and connectors to solve variations on the same class of problems.

Engineering is closer to applied science — there is a book of knowledge, a reference that guides the practice. Software has only heuristics. The IEEE tries; it doesn't quite get there.

The quality of the craft depends not on the quality of the tools but on the experience and intelligence of the craftsman. This is why good engineers can pick up any language quickly — all languages are semantic sugar over the same underlying constructs — and why bad engineers stay lost regardless of what stack they're handed.

This is also the argument against boot camps. A narrow training that doesn't expose someone to the underlying constructs produces a technician who won't learn beyond their initial toolkit. The CompSci degree teaches the abstraction layer that makes all subsequent learning faster.

---

## On Hiring

Engineering managers typically have no idea what they're looking for or how to find it, or both. Their reliance on "gut feel," "culture fit," and "I know what good looks like" is at best unteachable even when genuine, and most of the time is simple post-hoc rationalization. They could achieve equivalent outcomes by throwing dice and would save considerable time doing it.

They count as their success when strong candidates are hired, ignoring that the candidate self-selected into a job they could do and that the pipeline, not the interview loop, is what produced the option. Recruiting would make better decisions with less cost.

The corrective is structured competency frameworks with evidence requirements — "has done X, resulting in Y, measured by Z" — and AI-assisted evaluation that separates assessment from social dynamics. The bar-raiser function exists specifically to surface what the panel explained away.

---

## On the Leader/Manager Dichotomy

The Nibley leader/manager distinction is real but the dichotomy is *argumentum ad extremum*. Pure leaders — 100% leader, zero managerial capability — don't survive. They are the biblical prophets and apostles who ultimately pay with their lives for their inability to get on with the world. The gift and the fate are the same thing.

Pure managers are more common but without any leadership capacity they won't rise far. The inability to persuade includes the inability to persuade people to promote you.

Patton got to general. He still got through West Point. He still had something of the manager in him.

The interesting work — in real organizations and in the novel — is identifying the ratio in yourself and others. Not whether someone is a leader or a manager but at what proportion the leader quality becomes the fatal flaw. Harkovich's tragedy isn't that he's a leader. It's that the ratio left him with just enough managerial residue to survive but not enough to be contained by any institution that could have used him.

---

## On Theory of Constraints

TOC is a powerful tool with a specific failure condition: it breaks down when confronted with systemic reinforcing problems. When constraints are mutually reinforcing — when solving one strengthens the others — there is no single constraint to optimize or remove. All must be addressed simultaneously because partial solutions strengthen what remains.

The harder you push the system, the harder it pushes back. Senge's *Fifth Discipline* is the more useful frame here — stocks, flows, reinforcing loops, and the leverage points that are often counterintuitive. TOC's sequential logic is an elegant model for linear constraint systems. Real organizations are rarely linear.

---

## On What a Sr. Director Actually Does

Two versions of this misunderstanding:

**What the role is:** Poorly specified in most organizations. The working definition in practice is "a Director with more direct reports and higher compensation." Directors sit in offices waiting for problems to be brought to them and adjudicating those problems. That is the predominant model and it is wrong.

The right model is MacGregor — a 1995 *Organizational Dynamics* case study that has been in circulation for 23 years and shared with every team that could benefit from it. MacGregor runs the most efficient refinery in the corporation. He plays a lot of golf. He hasn't made an operating decision in years. His subordinates make decisions; he negotiates objectives, monitors Wednesday reports, and plans. His Thursday men consistently get promoted to run their own refineries. People read "lazy" until the results arrive. Then they read "lazy and lucky."

The actual cognitive work: develop people to the point where they don't need you for operational decisions, so you can think about what actually matters — the strategic fights that will determine the organization's position in two years, not this sprint.

**How the approach gets misread:** People mistake the problem being attacked for the identity of the person attacking it. If the current focus is hiring, the assumption is "this is a team builder." If the focus is project management, the assumption is "this is a PM." The actual logic is different.

Every tactical fight is also a strategic fight. A recent internal debate about disabling PAT tokens in JIRA was not about API access. It was about the right boundary between engineering autonomy and administrative centralization — about whether JIRA admins, ARBs, and CABs would continue to accumulate control that slows delivery. The PAT token was the surface. The fight was about all future fights of that type. Ender doesn't fight the bully to win that fight.

---

## On Who Gets Trust

Engineers, managers, peer directors — anyone — who will tell you to your face that you are wrong and engage in the debate. The position doesn't matter; the willingness to hold it in front of you does.

Quislings who agree to your face and whisper behind your back are useless. The information you need from them never reaches you. The dynamic they create in a team is corrosive. You can't manage what you can't see, and they make sure you can't see.

---

## On What Changed

Used to believe GenEd requirements for CompSci degrees were a waste of time. When boot camps emerged, believed the argument: who cares if a good programmer passed Art History or Fitness for Life?

Since reversed this on both counts.

On the CompSci side: boot camp graduates consistently demonstrate an unwillingness to learn beyond their initial training. The narrow scope isn't incidental — it's the product of training that never exposed them to the abstraction layer underneath. A CompSci degree teaches that all languages are semantic sugar. Boot camps teach a language. The difference compounds over a career.

On the liberal arts side: those courses don't benefit the programming at all. But they make a much better coworker. They teach people to read. They teach people to think critically. Most importantly — and this is the part that took time to see clearly — they make people human. Humane. A developer who has wrestled with literature, history, and philosophy has been asked to inhabit perspectives not their own. That capacity shows up in how they communicate, how they handle conflict, and whether they can work with people who are not like them. It is not a soft skill. It is the prerequisite for most of what makes an engineering team function.
