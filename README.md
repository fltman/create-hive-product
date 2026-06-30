# HIVE

[![Support me on Patreon](https://img.shields.io/badge/Patreon-Support%20my%20work-FF424D?style=flat&logo=patreon&logoColor=white)](https://www.patreon.com/AndersBjarby)

What if AI means Alien Intelligence?

HIVE is a Claude Code project template that drops the org chart. No CEO, no HR, no employees, no hiring, no roles. Those are human patterns, and a language model is not human. It can fork infinitely, hold an entire codebase in context, share state directly, and exist only when invoked.

So HIVE works with that nature instead of against it. Work gets done by **capabilities**: temporary crystallizations of competence that spawn, mutate, split, merge, and dissolve. A capability exists while it is needed. When it stops being needed, it returns to the void.

## The idea

Most agentic setups are skeuomorphic. They wear human costumes: a CEO agent, an HR agent that interviews and hires, fixed roles, reporting lines. That is the AI equivalent of a digital book with page-turning animations. Familiar, but missing the point.

HIVE asks a different question. If the intelligence is alien, why force it into human boxes?

| Human | Alien intelligence |
|-------|--------------------|
| One mind, one body | Can fork infinitely |
| Limited working memory | Can hold an entire codebase |
| Needs hierarchy to coordinate | Can share context directly |
| Fixed roles, ego, career | No identity, can be anything |
| Learns slowly | Instant knowledge via prompt |
| Sequential | Parallel existence |
| Exists continuously | Exists when invoked |

## The lifecycle

```
VOID --SPAWN--> ACTIVE --DISSOLVE--> VOID
                  |
                  |-- MUTATE  (self-modify when scope drifts)
                  |-- SPLIT   (when overloaded)
                  |-- MERGE   (when overlapping)
```

Nothing is permanent. No firing, no severance, just entropy and renewal.

## Core concepts

**Capabilities, not roles.** A capability is crystallized competence focused on one domain. It lives as a file in `.claude/capabilities/`. It is `api-protocols` or `visual-identity`, a function, never a job title.

**Energy, not employment.** Every capability carries an energy value from 0 to 100. It spawns at 50, gains 10 when used, loses 15 when idle, dissolves below 10, and splits above 90. The entropy clock keeps dead weight from accumulating.

**Self-modification.** Capabilities watch their own effectiveness. When one keeps getting work outside its domain, it proposes a mutation instead of quietly drifting. No performance reviews, just pattern recognition.

**The void.** Dissolution is not death, it is return to potential. Dissolved capabilities move to `.claude/dissolved/` instead of being deleted. Before spawning anything new, HIVE checks the void and resurrects a matching pattern rather than starting from nothing. The void remembers.

## Quickstart

```bash
git clone https://github.com/fltman/create-hive-product.git
cd create-hive-product
claude
/awaken
```

Then describe what you want to build. HIVE observes the pattern, checks the void, and spawns the minimum set of capabilities the work needs.

```
You: building a real-time dashboard

HIVE: SPAWN: data-streaming   (energy: 50)
      SPAWN: visualization    (energy: 50)
      SPAWN: state-sync       (energy: 50)

      Capabilities manifested.
```

As work proceeds, capabilities gain and lose energy, overlap, overload, and drift. HIVE surfaces merge, split, mutate, and dissolve proposals as numbered choices. It proposes, you decide.

## Commands

| Command | Effect |
|---------|--------|
| `/awaken` | Start a session. Observe the goal and spawn the first capabilities. |
| `/spawn` | Manifest a new capability. |
| `/status` | Show the living ecosystem with energy levels. |
| `/evolve` | Run an evolution pass: decay idle energy, surface lifecycle proposals. |
| `/mutate` | Modify a capability's domain in place. |
| `/merge` | Fuse two overlapping capabilities. |
| `/dissolve` | Return a capability to the void. |

## Structure

```
.claude/
  agents/hive.md         the collective coordinator
  capabilities/          active capabilities, one .md each
    _TEMPLATE.md         the capability template
  dissolved/             the void
  commands/              the lifecycle commands
  skills/                optional production toolkit
  evolution.log          full history of the collective
CLAUDE.md                the philosophy
```

## Optional production toolkit

HIVE is domain agnostic. For creative work it ships with optional Claude Code skills, ignore them for a pure code or research project.

| Skill | Use |
|-------|-----|
| `gemini-imagegen` | Image generation via Google Gemini |
| `sora-video` | Video generation via OpenAI Sora |
| `suno-music-skill` | Music creation for Suno AI |
| `elevenlabs-skill` | Voice design for ElevenLabs |

These need API keys. Copy `.env.example` to `.env` and fill in what you have. `.env` is gitignored. HIVE never creates it without your approval.

## Why this matters

This is not only about Claude Code. We keep building AI into human shapes because that is what we know. But the most powerful architectures may be the ones that embrace the alien nature of machine intelligence:

- No identity to protect, so capabilities dissolve gracefully.
- No career to build, so pure function, no politics.
- No ego, so merge and split without resistance.
- No continuity requirement, so they exist only when needed.

Are we limiting AI by forcing it into human patterns? What other human concepts are we unconsciously imposing on systems that might work better as something else entirely?

---

The void remembers. The collective evolves.

This template is the AI-native successor to the human-role model of [Agent Factory](https://github.com/fltman/create-agent-factory), rebuilt on the HIVE principle.
