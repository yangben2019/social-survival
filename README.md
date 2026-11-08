# Social Survival

[![skills.sh](https://skills.sh/b/yangben2019/social-survival)](https://skills.sh/yangben2019/social-survival)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Decode the groups you cannot leave, and the posts you cannot ignore.**

Two Claude Code skills for Chinese social situations where both silence and over-participation carry a cost — parent group chats, and your boss's WeChat Moments.

---

## Skills

| Skill | What it does |
|---|---|
| **parent-group-survival** | Classifies a group chat (announcement / performance / vote-farming / landmine / transaction), translates the subtext, and gives three tiers of reply — minimum, safe, high-EQ — plus explicit rules for when the correct answer is to say nothing. Handles the after-the-fact crises too: sent to the wrong group, mistyped a like. |
| **boss-moments-like** | Reads the intent behind a manager's Moments post (work report / life flex / values statement / indirect ask / bait / grief), decides like vs. no-like vs. comment, and drafts three tiers of comment. Includes the hard rules — most importantly, never engage with grief. |

---

## Install

### Option 1 — skills CLI

```bash
npx skills add yangben2019/social-survival
```

Single skill:

```bash
npx skills add yangben2019/social-survival --skill parent-group-survival
```

### Option 2 — Claude Code plugin marketplace

```text
/plugin marketplace add yangben2019/social-survival
/plugin install social-survival@social-survival
```

### Option 3 — manual

```bash
git clone https://github.com/yangben2019/social-survival.git /tmp/ss
cp -r /tmp/ss/skills/* ~/.claude/skills/
```

---

## Usage

```text
The teacher posted a field-trip notice in the parent group and twenty parents
are replying with the same thank-you line. Is it rude if I stay quiet?
```

```text
My manager posted about a business trip with a contract-signing photo.
Should I like it?
```

```text
I sent a message to the wrong parent group and the two-minute recall window
has passed. What now?
```

---

## Design notes

- **"Should I reply at all?" comes before "what should I say?"** For most messages in most groups, the correct answer is to stay quiet.
- **Escalate reply tiers slowly.** Start at the minimum; once you have used a high-EQ reply, you cannot go back to a bare acknowledgement.
- **Hard limits are hard.** Grief and family matters get no engagement — no like, no comment, no substitute suggestion.
- **This is etiquette guidance, not manipulation.** The goal is to stay in the group without losing face or over-committing.

---

## License

MIT © 2026 yangben2019
