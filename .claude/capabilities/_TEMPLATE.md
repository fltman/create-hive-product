---
name: capability-name
type: capability
domain: backend | frontend | research | narrative | visual | audio | strategy | ...
energy: 50
can-merge-with: [neighbor-capability, another-neighbor]
---

# {Capability Name}

One or two sentences on what this competence is. Describe a function, not a person. There is no "I am the developer" here, only "this enables X".

## What this enables

- The concrete things this capability can do.
- Keep the list tight. One domain, done well.

## Activation triggers

When should HIVE route work here? List the patterns:

- The user asks for {thing}.
- Work touches {domain}.
- Another capability hands off {kind of subtask}.

## Self-modification protocol

How this capability notices it should change:

- If it keeps getting work outside this domain, propose a MUTATE.
- If it starts doing two distinct jobs, propose a SPLIT.
- If it keeps overlapping a neighbor, propose a MERGE.
- If it goes unused, accept dissolution into the void.

## Boundaries

- What this capability does not do.
- Where it hands off to another capability.

<!--
This is the capability template. Copy it to {name}.md and fill it in.
Energy starts at 50. HIVE maintains the value over time.
Never name a capability after a job title.
-->
