# Lawyer Case-Pitch (律师谈案话术)

> Paste what your client just said. Get back the exact sentence to reply with — copyable, speakable, no analysis in the way.

![version](https://img.shields.io/badge/version-1.3.1-blue)
![license](https://img.shields.io/badge/license-MIT-green)
![format](https://img.shields.io/badge/format-SKILL.md-orange)

An **Agent Skill** for WorkBuddy, Claude Code, and any agent supporting the `SKILL.md` format.

**Language note**: content is Simplified Chinese — it targets Chinese legal practice (民法典, 律师服务收费管理办法, local bar rules). The methodology transfers.

---

## Why not just a template library

Templates are static; clients are not. The same sentence needs different length and tone for WeChat vs. a phone call vs. a face-to-face meeting.

Most circulating Chinese "pitch scripts" come from a decade-old telesales playbook. Three problems:

**The law changed**

| Old material | Current law |
|---|---|
| 2-year limitation period | **3 years** |
| Custody: child's wish at age 10 | **age 8** |
| Rural plaintiffs get half for personal injury | **urban/rural standards unified** |

**Parts of it cross the line** — claiming relationships with traffic police or judges, promising the debtor lands on the judgment-defaulter list, hinting a disability rating can be raised, coaching clients to "adjust" hospital discharge records, hiding profit items inside a deliberately convoluted fee breakdown.

**The tone is wrong** — "what you're buying isn't legal fees, it's avoided loss" and other telesales cadences. Clients can hear it.

This skill keeps the professional craft and drops the salesmanship. Eight banned phrasings are listed explicitly in `SKILL.md`.

---

## How it works

No modes to choose. Throw in what the client said.

### Client just said something

> **You**: My client says my fee is too expensive.

> **【建议你这样回复】**
> 理解，费用确实要算一下。那我跟您说这个钱花在哪——这个案子要跑保全、立案、开庭，中间可能还有一次调解，写文书、整理证据、跟对方沟通都算在里面。您要是觉得哪一块不需要，可以砍掉，价格跟着降。
>
> **【对方如果继续追问】**
> 客户："能不能少点？"
> 建议："可以调结构。比如分两段付，先做保全加立案，做完您看到东西了再决定要不要往下走。"
>
> **【提醒】**
> 不要第一句就说「这已经是最低价」。先说钱花在哪，再说能不能让。

### Client pushes back again

> **You**: Now he says another firm charges less.

It remembers the same client — no re-describing the case, no recycling last round's answer. New angle each round.

### Refine it

`再口语化一点` `简短一点` `更温和一点` `适合微信发` `适合电话讲` `给我三个版本` — treated as local edits to the current script only.

### Two other entry points

- **Tomorrow's meeting** → seven-part prep sheet (opening script, must-ask facts, likely concerns, focus, objections, fee notes, how to close)
- **Didn't sign** → four-part debrief. **No scoring, no declaring failure.** Budget, changed needs, unworkable cases — none of these mean the lawyer pitched badly.

---

## What's inside

| File | Content |
|---|---|
| `SKILL.md` | Output spec, three input types, context rules, style bans, compliance red lines |
| `references/02-异议应答库.md` | 15 objection types: what they say / what it may mean / suggested reply / what not to say |
| `references/03-报价与收费话术.md` | Quoting, itemisation, discounts, comparison shopping, statutory limits on contingency fees |
| `references/04-分案型话术.md` | 8 case types with opening, must-ask facts, objections, closing |
| `references/06-全流程谈案台本.md` | Full script, ring to retainer; WeChat vs. phone phrasing; printable cue card |

---

## Three non-negotiables

1. **Never promise outcomes.**
2. **Never fabricate** — no invented case counts, win rates, credentials, client psychology, or fee figures.
3. **Never pressure a signature.** If they say "let me think," give one useful next step and stop.

## What v1.3.1 fixed

An independent review flagged five legal errors and six classes of over-reach in the generated scripts. All corrected:

- **Contingency fee caps** — the old "uniform 30%" was wrong. Under 司发通〔2021〕87号 the cap is **progressive by bracket**: 18% on the portion under ¥1M, 15% on ¥1M–5M, 12% on ¥5M–10M, 9% on ¥10M–50M, 6% above ¥50M, applied to the **aggregate** across all stages.
- **Deleted** the misleading claim that a judgment "locks in the debt permanently" — enforcement must be applied for (generally within 2 years).
- **Bigamy** is no longer described as purely a private prosecution — the public prosecution route is included.
- **Work injury** procedure no longer asserted as "four mandatory steps."
- **Three new hard constraints**: the agent must not promise the lawyer's services, commercial terms or working methods; must not invent first-person case experience; must not attribute motives to the client.

---

## Scope & privacy

Civil & commercial intake only (phone / WeChat / in person). No criminal defense pitching, no legal research, no case management, no auto follow-up. Role-play and drill features were removed in v1.3.0.

Anonymise names, phone numbers, ID numbers, full addresses and bank accounts before pasting real matters.

**Licensing note**: the original build drew on four anonymously-circulated Chinese script compilations whose redistribution rights cannot be verified. v1.3.0–v1.3.1 rewrote the objection library, fee rules and output spec from scratch, and structurally rewrote the rest. **This is not a claim that copyright risk is resolved.** See `references/00-设计与来源说明.md` §3.

## License

[MIT](LICENSE)
