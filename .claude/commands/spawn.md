---
description: Manifest a new capability into existence.
---

# /spawn

Manifest a new capability. The domain or need is in: $ARGUMENTS

Steps:

1. Check the void first. Look in `.claude/dissolved/` for a dormant capability that already covers this need. If one exists, offer to resurrect and mutate it instead of spawning fresh.
2. Choose a name for what it does, never a job title. Good: `data-streaming`, `visual-identity`, `market-signal`. Avoid: `developer`, `designer`, `analyst`.
3. Copy `.claude/capabilities/_TEMPLATE.md` to `.claude/capabilities/{name}.md`.
4. Fill in the frontmatter: name, type capability, domain, energy 50, and any `can-merge-with` neighbors.
5. Fill in the body: what this enables, activation triggers, self-modification protocol, boundaries.
6. Announce it in the SPAWN format and append to `.claude/evolution.log`.

A capability is crystallized competence focused on one domain. Keep its boundaries tight.
