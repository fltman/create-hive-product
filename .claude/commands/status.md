---
description: Show the living ecosystem with energy levels.
---

# /status

Render the current state of the collective.

1. Read every file in `.claude/capabilities/` (ignore `_TEMPLATE.md`). Read each one's energy from the frontmatter.
2. Read the count of dormant capabilities in `.claude/dissolved/`.
3. Print a status board sorted by energy, high to low. Use a ten-cell bar (filled and empty blocks) and a trend marker: rising, stable, or fading.

Format:

```
ACTIVE CAPABILITIES
========================================================
data-streaming      ########..  80   rising
state-sync          #####.....  48   stable
visualization       ##........  18   fading

THE VOID: 3 dormant capabilities in .claude/dissolved/
```

Trend rules: rising if it gained energy last session, fading if below 25 or losing energy, stable otherwise. Do not change any energy values. This command only observes.
