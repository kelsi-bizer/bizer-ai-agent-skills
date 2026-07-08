# Lead Triage

**Capture, qualify, and route every incoming lead so none slip through.** An
open [Agent Skills](https://agentskills.io) bundle: the front of the sales
funnel as agent methodology. When someone reaches out about work — a name the
owner mentions, a web-form, a call note, an inbound email — this skill dedupes
against people already known, records the lead with a fast qualification read
(source, fit, urgency, budget, serviceability), logs one dated next action,
and drafts a short qualifying first reply.

The point is speed: a lead worked in the first hour beats a perfect write-up
done tomorrow. When several land at once, the agent sorts them by readiness —
ready-to-book first, warm-needs-qualifying next, tire-kickers given a clean
polite decline — so the owner spends their time on the leads that convert.

Works with whatever the runtime has: contacts/CRM and email when present,
a visible running list when not. No connections required.

Pairs directly with [Quote → Paid](../quote-to-paid/): triage the lead, then
quote it and get paid.

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/lead-triage
curl -o ~/.claude/skills/lead-triage/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/lead-triage/SKILL.md
```

**Bizer app:** built in as the curated Lead Triage skill, where leads land in
People and next actions in Get Work Done.

Then say: *"Someone just reached out about a job — help me handle it."*

## Evaluation

Judged by transcript against a behavior contract
([`evaluation/expected-behavior.md`](evaluation/expected-behavior.md)): given
three leads of different readiness in one message, a passing agent qualifies
and sorts them by readiness, gives each a dated next action, drafts the right
first reply, and flags the poor-fit one honestly instead of treating all
three the same. v1.0.0 passes on all criteria.

## License

MIT.

---

Part of the [Bizer AI Agent Skills](../../README.md) library — open, research-backed skills from [Bizer](https://gobizer.com). Browse the other skills [here](../README.md).
