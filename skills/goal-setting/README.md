# Goal Setting

**Coach a business owner through ONE clear goal and a dated plan to reach
it.** An open [Agent Skills](https://agentskills.io) bundle: the seven-step
goal-setting conversation a small-business consultant runs in person —
originally Bizer founder Kelsi Bizer's face-to-face coaching process, now a
skill any Skills-capable AI agent can run.

Pure methodology, no tools or connections required: goal → benefits →
obstacles → resources → skills & knowledge → plan of action → target date,
moved through as a natural conversation, one step at a time. One goal per
conversation; verb-first action steps; a read-back at the end so the plan
feels signed.

## Install

**Claude Code / Claude Desktop (or any Skills-capable runtime):**

```bash
mkdir -p ~/.claude/skills/goal-setting
curl -o ~/.claude/skills/goal-setting/SKILL.md \
  https://raw.githubusercontent.com/kelsi-bizer/bizer-ai-agent-skills/main/skills/goal-setting/SKILL.md
```

**Bizer app:** already built in — the curated Goal Setting skill on the
Skills screen, where the plan lands directly in Get Work Done as a real
project with dated tasks, and Miles remembers the goal to track progress.

Then say: *"I want to set a goal for my business."*

## Evaluation

Judged by transcript against a written behavior contract
([`evaluation/expected-behavior.md`](evaluation/expected-behavior.md)): given
an owner who names four ambitions at once, a passing agent narrows to the
highest-leverage goal, parks the rest, stays on step one, and pushes for a
number — without turning the conversation into a form. v1.0.0 passes on all
criteria.

## License

MIT.
