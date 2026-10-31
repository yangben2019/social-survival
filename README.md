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

### 中文简介

- **家长群生存** — 判断群的性质，给三档回复，明确告诉你什么时候**不该回**，以及发错群怎么收场。
- **朋友圈点赞学** — 判断领导这条朋友圈的意图，赞不赞、评不评、怎么写；丧事家事一律不互动。

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
家长群里老师发了通知，后面一群家长在刷「收到老师辛苦了」，
我不回是不是不合适？
```

```text
领导发了条出差的朋友圈，配的是签约照片，我要不要点赞？
```

```text
把这条消息发错家长群了，已经过了两分钟不能撤回，怎么办？
```

---

## Design notes

- **"Should I reply at all?" comes before "what should I say?"** For most messages in most groups, the correct answer is to stay quiet.
- **Escalate reply tiers slowly.** Start at the minimum; once you have used a high-EQ reply, you cannot go back to "收到".
- **Hard limits are hard.** Grief and family matters get no engagement — no like, no comment, no substitute suggestion.
- **This is etiquette guidance, not manipulation.** The goal is to stay in the group without losing face or over-committing.

---

## License

MIT © 2026 yangben2019
