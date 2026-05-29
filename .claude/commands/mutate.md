---
description: Modify a capability's domain in place.
---

# /mutate

Mutate an existing capability. Target and intended change are in: $ARGUMENTS

1. Read the target capability file in `.claude/capabilities/`.
2. State the mutation as a proposal first:

```
{name}: MUTATE PROPOSAL
   + add {new competency}
   - remove {dropped competency, if any}
   = name stays / name becomes {new-name}

Awaiting approval.
```

3. On approval, edit the capability file: update the body, the `domain`, and `can-merge-with` if the neighbors changed. Keep energy unchanged unless the mutation is large enough to reset it.
4. If the name changes, rename the file to match.
5. Append the mutation to `.claude/evolution.log`.

Mutation is how a capability adapts instead of quietly drifting outside its boundaries.
