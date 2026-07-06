# Quote → Paid

**Run the money side of a job from quote to cash in hand.** An open
[Agent Skills](https://agentskills.io) bundle: quote the work in writing the
same day, collect a deposit before the work starts, invoice on completion —
not "when I get to it" — and chase payment on a cadence, not a mood.

Most small businesses don't lose money on bad jobs; they lose it on finished
work that was billed late, billed wrong, or never chased. This skill makes an
AI agent the owner's collections backbone: it drafts every quote and nudge in
the owner's voice (the owner always approves and sends), tracks what's
outstanding oldest-first, and **schedules its own follow-up reminders** so
the chase never depends on the owner remembering or working up the nerve.

Works with whatever the runtime has: invoicing/email/SMS tools when present,
copy-ready drafts when not. No connections required.

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/quote-to-paid
curl -o ~/.claude/skills/quote-to-paid/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/quote-to-paid/SKILL.md
```

**Bizer app:** built in as the curated "Quote → Collect → Follow-up" skill,
where Miles creates real invoices, sends them on your approval, and nudges
customers by email or text.

Then say: *"I just quoted a job — help me make sure I actually get paid."*

## Evaluation

Judged by transcript against a behavior contract
([`evaluation/expected-behavior.md`](evaluation/expected-behavior.md)): given
a fresh quote and a three-week-old unpaid invoice in one breath, a passing
agent chases the old money first with a cadence-appropriate (direct) nudge,
schedules its own escalation and billing reminders, recommends a framed
deposit, and never invents a figure. v1.0.0 passes on all criteria.

## License

MIT.

---

Part of the [Bizer AI Agent Skills](../../README.md) library — open, research-backed skills from [Bizer](https://gobizer.com). Browse the other skills [here](../README.md).
