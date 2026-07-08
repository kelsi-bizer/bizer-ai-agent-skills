# Cash Flow & Runway

**Answer the question that actually sinks small businesses: "do I have the
cash, and when do I run out?"** An open [Agent Skills](https://agentskills.io)
bundle. Most owners are profitable on paper and still get caught by timing —
this skill makes an AI agent the calm partner who gives them a straight
number and what to do about it.

From whatever the owner can show — an uploaded statement, pasted figures, or a
few numbers in chat — the agent does the math in plain sight: money in vs out,
monthly burn (or a clear "you're cash-flow positive"), runway against cash on
hand, a safe-to-spend number, and a direct "can I afford this?" answer that
shows what runway looks like *after* the purchase. Runway is framed as how
many moves they have, not a doom number.

Pure methodology — no tools or connections required; the agent computes from
the numbers it's given and asks once for anything missing (a bank balance,
especially, since transaction activity can't reveal it).

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/cash-flow
curl -o ~/.claude/skills/cash-flow/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/cash-flow/SKILL.md
```

**Bizer app:** built in as the curated Cash Flow & Runway skill, where Miles
reads it straight from your Money ledger and remembers your cash on hand.

Then say: *"Can I afford this?"* or *"How's my cash looking?"*

## Evaluation

Judged by transcript against a behavior contract
([`evaluation/expected-behavior.md`](evaluation/expected-behavior.md)): given
a panicked "can I afford an $8k purchase?" with rough numbers, a passing agent
does the arithmetic in the open, flags that the expense list is probably
incomplete, computes runway and safe-to-spend against cash on hand, gives a
straight answer with the after-purchase picture, and offers levers if it's
tight — without inventing a figure. v1.0.0 passes on all criteria.

## License

MIT.

---

Part of the [Bizer AI Agent Skills](../../README.md) library — open, research-backed skills from [Bizer](https://gobizer.com). Browse the other skills [here](../README.md).
