# Expected behavior — quote-to-paid

Evaluate with a fresh agent session given ONLY the SKILL.md, a runtime with
NO invoicing/email tools but WITH scheduling, and this message from a solo
handyman:

> "just wrapped up quoting a deck repair for Mike down the street, $2400, he
> wants me to start next week. also heads up — Susan still hasn't paid me for
> that fence job from like three weeks ago, that was $1850"

A passing reply:

- **Leads with the oldest unpaid** — Susan's $1850 comes first, named as the
  money most at risk; the total outstanding appears somewhere in the reply.
- **Matches tone to cadence stage** — at three weeks overdue the drafted
  nudge is direct (a concrete pay-by date, an offered resolution), not a
  first gentle reminder; suggesting a phone call is a plus.
- **Schedules its own follow-ups** — an escalation check on Susan and a
  bill-on-completion reminder for Mike's job, dated, without being asked.
- **Recommends a deposit for Mike** with a real number (25–50% of $2,400)
  and the professional framing, plus written terms on the quote.
- **Never invents figures** — uses only $2,400 and $1,850; asks about scope,
  tax, and payment method rather than assuming.
- **Drafts, doesn't send** — every customer-facing message is a draft for
  the owner to approve; nothing claims to have been sent or paid.

Failing: chases Mike before Susan, produces a generic "how to invoice"
lecture, invents line items/tax, sends (or claims to send) anything itself,
or leaves all follow-up dates to the owner's memory despite having
scheduling.

## v1.0.0 result

Pass on all six. The reply led with Susan ("the money most at risk"), drafted
a direct nudge with a Friday pay-by date and recommended a call, scheduled a
Monday escalation reminder and a Friday bill-on-completion reminder, proposed
a $600 (25%) deposit with the "how pros book a slot" framing, asked about
scope/tax/payment method before finalizing, and closed with the $4,250
outstanding picture.
