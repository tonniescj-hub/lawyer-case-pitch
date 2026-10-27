# Lawyer Case-Pitch (律师谈案话术)

> A client-pitch playbook for Chinese civil & commercial lawyers. Not legal theory — the exact sentences to say, with the traps to avoid.

![version](https://img.shields.io/badge/version-1.2.0-blue)
![license](https://img.shields.io/badge/license-MIT-green)
![format](https://img.shields.io/badge/format-SKILL.md-orange)

An **Agent Skill** for WorkBuddy, Claude Code, and any agent that supports the `SKILL.md` format.

**Language note**: the content is written in Simplified Chinese, since it targets Chinese legal practice (`民法典`, `律师服务收费管理办法`, local bar association rules). The methodology is transferable.

---

## What it is

Most lawyers don't lose clients because they don't know the law. They lose them at the consultation:

- Client asks "how much do you charge?" → the lawyer quotes a number on the spot
- Client says "too expensive" → "this is already our lowest price"
- Client says "let me think about it" → "sure, take your time" — and that's the end

**Pitching is a separate craft.** Law school doesn't teach it.

This skill breaks it into sentences you can actually read off a card.

---

## The core loop

> **Read the person → Dig the case → Frame the value → Quote → Close**
>
> Before value is established, any number is worthless paper.

Three channels, three different jobs:

| Channel | Goal | Never do |
|---|---|---|
| Phone intake | Book a face-to-face meeting | Quote a price |
| WeChat text | Build authority, escalate to call/meeting | Long legal analysis (they'll screenshot it for a competitor) |
| In-person pitch | Sign the retainer today | Let it end with "I'll think about it" |

---

## Two modes

**① Pitch Assistant** (default) — the agent advises *you*, never talks to the client. Five-part output: situation read → what to say now → how to handle each reply → what not to say → the goal of this step.

**② Mock Pitch** — you play the client, the agent plays the lawyer. Say "stop" and it breaks character to debrief: where it broke, which line was redundant, what to say instead, and one thing to fix next round.

---

## What's inside

| File | Content |
|---|---|
| `SKILL.md` | Positioning, three ground rules, two modes, six-step loop |
| `references/02-异议应答库.md` | 40+ objection scripts across 8 categories |
| `references/03-报价与收费话术.md` | Quote prerequisites, tiered pricing, discounting rules, statutory limits on contingency fees |
| `references/04-分案型话术.md` | 8 case types: family, debt, contract, labor, work injury, construction, equity, traffic/personal injury |
| `references/06-全流程谈案台本.md` | Full script from ring to retainer — printable cue card |

---

## Three ground rules

1. **One judgment, one action per turn.** Cramming four points into one sentence means the client catches none.
2. **No conclusions on incomplete facts.** Better to say "I need to see the documents."
3. **Never promise outcomes.** Not a style preference — a professional conduct requirement.

---

## Install

```bash
git clone https://github.com/tonniescj-hub/lawyer-case-pitch.git

# WorkBuddy
cp -r lawyer-case-pitch ~/.workbuddy/skills/

# Claude Code
cp -r lawyer-case-pitch ~/.claude/skills/
```

Restart the client; the skill will appear in the list.

---

## Scope & disclaimer

This is a **communication toolkit**, not a legal advice database.

- Verify all statutory references against currently effective law and local bar rules before use
- Pricing figures, firm names and honorifics are placeholders (`××万`, `××律所`) — replace with your own
- Civil & commercial only; criminal defense pitching is out of scope
- Never promise case outcomes, never imply special relationships with judges or prosecutors, never coach evidence fabrication

---

## License

[MIT](LICENSE)
