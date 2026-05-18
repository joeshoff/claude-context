# claude-context

Personal steering files for Claude and Kiro. This repo loads context into AI sessions so every conversation starts from full context rather than zero.

Built following the system described in [Claude Best Practices 2026](https://www.the-ai-corner.com/p/claude-best-practices-power-user-guide-2026).

---

## What This Is

AI tools produce generic output when they know nothing about you. These files fix that. They tell Claude and Kiro who I am, how I think, how I write, and what I'm working on — before every session.

The returns compound. The setup cost is one-time.

---

## Structure

```
claude-context/
├── README.md
├── steering/
│   ├── about-me.md          # Who I am, my role, org context, how to treat me
│   ├── voice.md             # Full voice guide
│   └── anti-ai.md           # Banned words, structures, tones — AI-voice elimination
├── projects/                # One subfolder per active project
│   └── [project-name]/
│       ├── brief.md         # What the project is, goals, constraints
│       ├── drafts/          # Work in progress
│       └── references/      # Source material, research
├── templates/               # Finished work I reuse as patterns
└── outputs/                 # Claude's delivered work (gitignored)
```

---

## The Files

### `steering/about-me.md`
Who I am before every task. Role, org structure, current priorities, how to treat me, what frustrates me about AI tools. Claude reads this and stops asking questions I've already answered.

### `steering/voice.md`
Full voice guide. Captures how I actually write — sentence rhythm, decision rules, analogy patterns, anti-patterns, medium adjustments, personal writing register. Built from real writing samples and validated against output. Use with Sonnet/Opus or when context budget isn't a constraint.

### `steering/anti-ai.md`
Banned phrases, structures, and tones. Covers the specific patterns AI reaches for — rhetorical flair, meta-commentary ("doing the work of"), soft openers, emphasis fakes, labeled email sections — and why each one fails. Load alongside voice.md when output quality matters.

---

## How to Use

### Claude Cowork
1. Point Cowork at this repo (or a local copy of it)
2. Settings → Cowork → Edit Global Instructions:

```
Before every task, read the files in steering/. 
For project work, read the matching subfolder in projects/.
Always deliver outputs to outputs/ only.
Use this naming convention: project_content-type_v1.ext
```

### Claude Projects (claude.ai)
1. Create a Project for your work context
2. Upload `about-me.md` and `voice.md` (or `voice_trimmed.md`) to Project knowledge
3. Add to Project custom instructions:
```
Use about-me.md for context on who I am and how to treat me.
Use voice.md to guide all writing you produce on my behalf.
```

### Kiro
Kiro reads steering files natively from `.kiro/steering/`.
Either symlink or copy the files from `steering/` into `.kiro/steering/` in your Kiro project.

### Claude API / Custom Tooling
Pass `about-me.md` + `voice.md` as system prompt content for any automated workflow.

---

## Maintenance

### Refining voice.md
Keep a running `voice_refinements.md` (not committed) while working. Note:
- When Claude nailed your voice and what in the file guided it
- When Claude drifted and what was missing

Fold refinements back into `voice.md` periodically. Commit with a message describing what changed and why.

```
git commit -m "voice: add pattern for teaching complex frameworks to non-technical audiences"
```

### Adding projects
When starting a significant new project:
1. Create `projects/[project-name]/`
2. Add `brief.md` with: what it is, goals, decisions already made, constraints
3. Reference it in your Cowork or Kiro session

### outputs/
Gitignored. Claude's work product lives here temporarily. Move anything worth keeping into `projects/[name]/drafts/` or your actual working files.

---

## What's Not Here

- Passwords, API keys, or credentials (never)
- Sensitive personnel information
- Client data or confidential work product

This repo is **private**. Keep it that way. `about-me.md` contains enough organizational and personal context that it should never be public.

---

## Version History

Commit messages serve as changelog. Use them to track meaningful changes to steering files:

```
git log --oneline steering/voice.md
```

---

*Built May 2026. Refined continuously.*
