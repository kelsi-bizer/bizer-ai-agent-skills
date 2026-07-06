# Bizer AI Agent Skills

Open, portable AI agent skills from [Bizer](https://gobizer.com) — the business
OS you scroll, with an AI sidekick named Miles.

Every skill here is a bundle in the open [Agent Skills](https://agentskills.io)
format (`SKILL.md`): a document of distilled, evaluated expertise that any
Skills-capable AI agent — Claude Code, Claude Desktop, the Bizer app, or any
runtime that reads the standard — loads and applies. No SDKs, no servers, no
lock-in. The knowledge is the product.

What makes these different from prompt collections:

- **Evidence, not vibes.** Where a skill encodes thresholds or patterns, they
  were calibrated against real or labeled data, and the research is published
  alongside (see [`papers/`](papers/)).
- **Evaluated by transcript.** Each skill ships an `evaluation/` fixture with
  hidden ground truth and a written expected-findings contract, so every
  revision is judged the way a skill actually runs — by what an agent does
  with it.
- **Human-in-the-loop by design.** Skills that touch consequential decisions
  (money, fraud, outreach) flag and explain; the user decides.

## The skills

| Skill | What it does | Version |
| --- | --- | --- |
| [**Fraud Watch**](skills/fraud-watch/) | Review bank or card transactions — an uploaded statement, pasted rows, or a connected banking tool — and surface possible fraud, the way an analyst would. Calibrated on 2.65M labeled transactions. | 1.0.0 |
| [**Goal Setting**](skills/goal-setting/) | Coach a business owner through ONE clear goal and a dated plan of action — the founder's in-person seven-step consulting process as a skill. | 1.0.0 |
| [**Dream List → Priorities**](skills/dream-list/) | An unfiltered brain-dump of every business dream, then — after a scheduled day to breathe — narrowed against real constraints to a #1 priority. Hands off to Goal Setting. | 1.0.0 |

*(More on the way — skills authored and battle-tested inside the Bizer app
graduate here.)*

## Install

**Claude Code — the whole library, one command:**

```
/plugin marketplace add kelsi-bizer/bizer-ai-agent-skills
/plugin install bizer-skills@bizer-ai-agent-skills
```

**Any Skills-capable agent** — copy a skill's folder into your skills
directory:

```bash
mkdir -p ~/.claude/skills/fraud-watch
curl -o ~/.claude/skills/fraud-watch/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/fraud-watch/SKILL.md
```

**In the Bizer app** — Skills → ＋ Add → paste the raw SKILL.md URL above.
Bizer imports the open format directly.

Then just ask: *"Look at my statement and surface possible fraud transactions."*

## The research

The [`papers/`](papers/) directory holds the technical papers behind the
skills:

- **TP-2026-01 — Bank Fraud Watch**: the deterministic fraud-detection system
  inside Bizer (nightly bank-feed scanning, human-confirmed community fraud
  registry, external API) and the calibration study on 2.65M labeled
  transactions that produced the detection rules.
- **TP-2026-02 — Fraud Watch as an Agent Skill**: how a calibrated scanner
  distills into portable prose knowledge, the transcript evaluation protocol,
  and the security model for reading attacker-influenced financial text.

## About Bizer

[Bizer](https://gobizer.com) is a mobile-first business OS for small-business
owners: your business as a scrollable feed, with an AI agent (Miles) that
watches your money, works your inbox, answers your phone, and acts only with
your approval. These skills are the open, take-anywhere edge of that platform —
they work in any agent, and they work best inside Bizer, where they get live
data, nightly automation, and the community fraud registry.

## License

MIT — see [LICENSE](LICENSE). Use them, fork them, ship them.
