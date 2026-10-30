# Web Summit Lisbon 2026 skill for AI assistants

Turn Claude (or any assistant that supports Agent Skills) into an expert navigator for **Web Summit Lisbon 2026** (9–12 Nov, MEO Arena and FIL) and **Web Summit Week / Portugal Tech Week** (6–15 Nov).

Ask in your own words and get answers that fit your goals:

- **A plan for your week**: tell it what you're building, who you want to meet and which evenings you're free. You get a day-by-day plan with one main side event and one backup per evening.
- **First-timer logistics**: badge pickup, airport to MEO Arena by metro, wifi and eSIM, luggage lockers at Oriente, coworking nearby, the First Timers meetup.
- **Side events by goal** (fundraise, build with AI, find peers, first-time orientation), each with date, Lisbon time, access type (free, paid, approval), clashes and the organizer's own link.
- **Night Summit or a side event?**, investor events you can apply to, and following up after the event.

It answers from Bebb's unofficial guides, the [Newcomer Antiguide](https://usebebb.com/websummit/newcomers) and the [Networking & Side Events Playbook](https://usebebb.com/websummit/networking). It names its sources and doesn't make things up. When the assistant has web access, it checks the live guides first, because they're updated daily during the week.

## Try it

```
First Web Summit! I build B2B AI tools, land Sunday evening, free Mon–Wed evenings.
I want design partners and to meet other AI founders. Plan my week?
```

```
We're raising a seed round. Which investor side events can I still apply to,
and what clashes with Venture Night?
```

```
quick one: does my ticket get me into side events? where do I pick up my badge?
```

## Install

### Claude app (web or desktop), about 1 minute

1. **[Download web-summit-lisbon-2026.skill](https://github.com/patnorris/usebebb-web-summit-week-lisbon-2026-companion-claude/releases/latest/download/web-summit-lisbon-2026.skill)**
2. In Claude, open **Customize → Skills**, click **+**, then **Create skill → Upload a skill**, and choose the downloaded file.
3. Make sure **Code execution and file creation** is turned on in Settings (skills need it).
4. Start a new chat and ask anything about Web Summit Week.

Custom skills are available on Pro, Max, Team and Enterprise plans. Skills you add in the Claude app also load in Claude Code when you're signed in with the same account.

### Claude Code

```
/plugin marketplace add patnorris/usebebb-web-summit-week-lisbon-2026-companion-claude
/plugin install web-summit-lisbon-2026@bebb
```

### Codex, Cursor, Gemini CLI, GitHub Copilot and other agents

Copy `skills/web-summit-lisbon-2026/` into your agent's skills folder. It follows the open `SKILL.md` format.

### No skill support?

Paste the guide straight into any assistant: [Newcomer Antiguide for AI](https://usebebb.com/websummit/newcomers/ai) · [Networking Playbook for AI](https://usebebb.com/websummit/networking/ai)

## What's inside

```
skills/web-summit-lisbon-2026/
├── SKILL.md                              # how the assistant plans and answers
├── references/
│   ├── logistics.md                      # arrival, badge, metro, wifi, luggage, coworking
│   └── networking-and-side-events.md     # curated side events, clashes, investor events, follow-up
└── evals/                                # test cases (run with `claude plugin eval`)
```

## Ground rules the skill follows

- **Sources first.** Answers come from the guides, with the official or organizer link.
- **Side events are a dated snapshot** (checked 27 Oct 2026). The organizer's page is the source of truth; the skill tells you to confirm there before you commit.
- **No promises.** It never says a specific person will attend or meet you, and never treats an RSVP as an approval.
- **Lisbon time** (WET, UTC+0) throughout.

## Freshness

Snapshot: guides last updated 29 Oct 2026. Updated releases follow during Web Summit Week. With web access, the assistant fetches the live guides for time-sensitive questions.

## Disclaimer and privacy

Unofficial. Bebb is not affiliated with Web Summit and this is not an official Web Summit service. For tickets, check-in and the official schedule, use the [official Web Summit app](https://websummit.com/app/). Side events need their own registration with each organizer.

The skill itself collects no data. It is instructions and reference text only. When the assistant has web access, it may fetch public pages on usebebb.com and the organizer sites it links to. Bebb's optional networking space is opt-in. See the [Bebb privacy policy](https://usebebb.com/privacy).

## Contributing

Spotted an outdated time, a broken link or a great side event that's missing? [Open an issue](https://github.com/patnorris/usebebb-web-summit-week-lisbon-2026-companion-claude/issues) with the organizer's link.

## License

[MIT](LICENSE) © 2026 Bebb
