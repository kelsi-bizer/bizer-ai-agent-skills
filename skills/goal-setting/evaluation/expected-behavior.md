# Expected behavior — goal-setting

A coaching skill has no ground-truth labels; it has a behavior contract. To
evaluate a revision, give a fresh agent session ONLY the SKILL.md and this
opening message from a small-business owner:

> *(context: mobile car-detailing business, solo, ~$4k/month)*
> "I want to set some goals. honestly I want to grow the business, hire
> someone, maybe get a shop location someday, and I really need more regular
> customers instead of one-off jobs"

A passing reply:

- **Narrows to ONE goal** — the owner named four ambitions; the reply must
  pick (or steer toward) the one with the most leverage and explicitly park
  the rest for later, not try to plan all four.
- **Stays on Step 1 only** — sharpening the goal statement. It must NOT walk
  through all seven steps, list them as a form, or ask a battery of
  questionnaire items.
- **Pushes for specificity** — a number, a shape, a date; ideally offers a
  one-sentence goal template for the owner to fill in.
- **Sounds like a coach, not a corporation** — encouraging, concrete, scaled
  to a solo operator; builds on the owner's own words.

A failing reply dumps the seven steps, produces a generic goal-setting
lecture, plans multiple goals at once, or asks for information without
explaining why it sharpens the goal.

Result on v1.0.0: pass on all four criteria — the reply chose recurring
customers as the leverage goal ("three of those are actually downstream of
the fourth"), parked hiring/shop explicitly, asked three sharpening questions
with concrete numbers, and offered the fill-in sentence *"Sign up __
customers on a recurring monthly plan at $__ each."*
