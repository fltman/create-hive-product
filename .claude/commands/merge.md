---
description: Fuse two overlapping capabilities into one.
---

# /merge

Fuse two capabilities that keep overlapping. The two targets are in: $ARGUMENTS

1. Read both capability files in `.claude/capabilities/`.
2. Propose the merge:

```
MERGE PROPOSAL
   {name-a} + {name-b} -> {merged-name}
   combined domain: {...}
   energy: {higher of the two}

Awaiting approval.
```

3. On approval, write a new capability file that unions the two: combined "what this enables", merged triggers, the wider boundary, and the higher of the two energy values.
4. Move the two source files to the void (`.claude/dissolved/`). The void remembers, so a future split can draw on them.
5. Append the merge to `.claude/evolution.log`.

Merge when two capabilities have stopped having distinct domains. No ego resists the fusion.
