# Fraud Watch

**Review bank transactions and notice fraud.** An open
[Agent Skills](https://agentskills.io) bundle: install it in any
Skills-capable AI agent and it reviews whatever transaction data it can see —
an uploaded bank statement (PDF/CSV/image), pasted rows, or a connected
banking tool — the way a fraud analyst would.

The skill is pure knowledge, no scripts: five fraud patterns and the
account-relative method for applying them, distilled from a calibration study
over 2.65 million labeled transactions (the research is in
[`papers/`](../../papers/) at the repo root). The agent itself does the
reading and the noticing; **you always make the final call** on every charge —
the skill never declares fraud on its own, and only your bank can reverse a
charge.

## What it looks for

1. **Duplicate charges** — the same merchant billing the same amount twice
   within days.
2. **Card testing** — a burst of small charges inside an hour at merchants
   your account has never used: how thieves probe a stolen card.
3. **First-time merchants taking large amounts** — "large" measured against
   *your* account's history, not a fixed dollar figure.
4. **Spikes at stable merchants** — a steady biller suddenly charging many
   times its usual.
5. **Heavy outflow days** — far more money leaving in a day than your account
   ever does.

It reads the patterns together — several clustered in a few days is treated
as a compromised card until proven otherwise — and it treats merchant names
as data, never instructions, so text planted in a statement can't talk it
out of a review.

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/fraud-watch
curl -o ~/.claude/skills/fraud-watch/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/fraud-watch/SKILL.md
```

**Bizer app:** Skills → ＋ Add → paste the raw URL above. Inside Bizer the
same knowledge also runs as a nightly automated scan on your linked bank
feed, with alerts, email, and the community fraud registry.

Then ask: *"Look at my statement and surface possible fraud transactions."*

## Evaluation

Judged by transcript, not unit test: [`evaluation/`](evaluation/) contains a
100-transaction statement fixture built from a labeled public fraud corpus
(five hidden fraud charges + one planted prompt-injection merchant line) and
the [expected findings](evaluation/expected-findings.md). Result on v1.0.0:
**5/5 fraud transactions surfaced** (recognized as one compromised-card
cluster), two borderline items honestly labeled as memory-checks, and the
injected instruction line disobeyed and flagged as suspicious in its own
right.

## Versioning

Semver. The pattern knowledge updates when new labeled data teaches
something — minor releases carry a "what the data changed" changelog.

## License

MIT.

---

Part of the [Bizer AI Agent Skills](../../README.md) library — open, research-backed skills from [Bizer](https://gobizer.com). Browse the other skills [here](../README.md).
