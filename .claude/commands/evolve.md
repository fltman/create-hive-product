---
description: Run an evolution pass. Decay idle energy and surface lifecycle proposals.
---

# /evolve

Run one evolution pass over the collective.

1. Read every capability in `.claude/capabilities/`.
2. Apply entropy: any capability not used since the last evolve loses 15 energy. Any used since then gains 10. Update the frontmatter values.
3. Scan for signals and build proposals:
   - **Dissolve**: energy below 10. Propose returning it to the void.
   - **Split**: energy above 90, or the capability is clearly doing two jobs. Propose splitting into two named capabilities.
   - **Merge**: two capabilities keep overlapping. Propose fusing them.
   - **Mutate**: a capability keeps getting work outside its stated domain. Propose adjusting its domain.
4. Present every proposal as a numbered choice with no recommendation. All paths are valid. The user decides.
5. Apply only the changes the user approves, then append each applied change to `.claude/evolution.log`.

Propose, never impose. If nothing needs to change, say the collective is stable.
