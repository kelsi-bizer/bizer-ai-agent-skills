# Dream List → Priorities

**Turn everything a business owner wishes for into a short list of clear
priorities.** An open [Agent Skills](https://agentskills.io) bundle: the
two-session consulting exercise Bizer founder Kelsi Bizer runs with
small-business owners in person — dream wide, then narrow — as a skill any
Skills-capable AI agent can run.

**Session one** is an unfiltered brain-dump: everything they need, want, and
dream of, as if money were no object, captured somewhere the owner can see —
and then the agent **schedules the review itself** (a day or two out, using
whatever reminders/scheduling the runtime offers), because owners always
remember more the next day. **Session two** weighs the list against real
constraints — money, time, and energy are objects now — and sorts it: a #1
priority with the leverage argument, near-term items kept warm, dreams parked
on a Someday list (parked, never deleted). Then it deliberately stops and
hands the #1 to goal planning — pairs directly with the
[Goal Setting](../goal-setting/) skill, which takes exactly that handoff.

Pure methodology: no tools or connections required; task and scheduling tools
are used when the runtime has them.

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/dream-list
curl -o ~/.claude/skills/dream-list/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/dream-list/SKILL.md
```

**Bizer app:** already built in — the curated "Dream List → Priorities" skill
on the Skills screen, where every item lands in Get Work Done as a real task
and Miles schedules the review and can put it on your calendar.

Then say: *"I have too many ideas — help me figure out what matters most."*

## Evaluation

Judged by transcript against a two-part behavior contract
([`evaluation/expected-behavior.md`](evaluation/expected-behavior.md)):
session one must capture without filtering and schedule the follow-up itself;
session two must sort against the owner's real constraints and stop at the
goal-planning handoff instead of building the plan. v1.0.0 passes both.

## License

MIT.
