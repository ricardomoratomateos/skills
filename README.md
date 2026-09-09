# The Skills Foundry

> Where agents stop improvising and start practicing a craft.

A prompt tells an agent what to want. A **skill** tells it how to work: the method, the
discipline, the rules it is not allowed to break. This repository is my growing collection of
battle-tested agent skills — each one distilled from real production use, stripped of every
trace of the application it was born in, and rebuilt as a portable, reusable craft.

No frameworks. No SDKs. Just markdown that turns a capable agent into a disciplined
practitioner.

## The doctrine

Every skill in this foundry obeys three laws:

1. **Generic by construction.** A skill describes *how to decide*, never *what things are
   called*. Anything that names a domain, a URL or a class is configuration, and configuration
   lives outside the skill.
2. **Evidence over confidence.** A skill never lets the agent claim what it did not observe.
   Verdicts are earned with screenshots, network captures and logs — or they are not verdicts.
3. **Autonomous and honest.** Where a human would ask a question, a skill takes the conservative
   path and records exactly what it could not do. An honest "pending" beats a fabricated "done",
   every single time.

## The collection

### `qa/` — the autonomous QA engineer

Four skills that together review a pull request the way a meticulous QA human would: log in,
read the PR, seed real data through the real API, drive the browser, capture evidence, deliver
a verdict, and remember what was learned for next time.

| Skill | Role |
|---|---|
| [`qa-login`](qa/qa-login/SKILL.md) | Opens the door. Per-environment authenticated sessions, SSO detection, zero guessing. |
| [`qa-prepare`](qa/qa-prepare/SKILL.md) | Turns a PR into an executable plan: flows, real endpoints, seeded data. |
| [`qa-execute`](qa/qa-execute/SKILL.md) | Drives the flows, captures the evidence, writes the report. The verdict machine. |
| [`qa-memory`](qa/qa-memory/SKILL.md) | Closes the loop: what this run learned, the next run inherits. |

Read the [pipeline documentation](qa/README.md) for the full method — the container contract,
the verdict semantics and the rules that are not up for negotiation.

## The roadmap

The foundry is open for business and the anvil is warm. QA is the first discipline forged
here; it will not be the last. More crafts are on their way.

## License & provenance

These skills were extracted from real systems and deliberately anonymized: no client names, no
domains, no credentials, no war stories with identifiable casualties. What remains is the part
that was always worth keeping — the method.
