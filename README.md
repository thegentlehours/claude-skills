# 5 free Claude skills for people who write, post and sell

Installable Agent Skills. Each one is a written procedure Claude follows when the task
matches: what to ask for first, the steps in order, the output format, and what it may
not make up. Each one also ends with the conditions under which it is the wrong tool.

| Skill | Use it when | One place it breaks |
|---|---|---|
| [Voice Check](skills/voice-check/SKILL.md) | A draft reads as AI-written and you can't say why | On text under ~150 words there is not enough material for variance analysis, and it will report tells that are just the length. |
| [Claim Auditor](skills/claim-auditor/SKILL.md) | Before you publish anything with a number in it | It cannot verify anything. It sorts claims by whether evidence exists; it cannot tell you whether your evidence is any good. |
| [Repurpose Content](skills/repurpose-content/SKILL.md) | One good piece should have been five | Thin sources. A 400-word post does not contain a week of content, and pretending it does produces five weak posts instead of one good one. |
| [Social Carousel](skills/social-carousel/SKILL.md) | You need a deck that earns a save | Text-heavy slides fail on mobile. If a slide will not read at thumbnail size, it is not a slide, it is a paragraph. |
| [Newsletter Issue](skills/newsletter-issue/SKILL.md) | It's send day and you want next week's open too | It cannot know what the list already received. Repeating an idea from three weeks ago is invisible to this skill and obvious to a subscriber. |

Every skill's full list of failure conditions is in its own `SKILL.md`.

## Installing

1. Download this repo, or copy the folder of the skill you want from `skills/`.
2. In Claude, open **Settings → Capabilities** and make sure Skills are enabled.
3. Go to **Skills** and upload the skill's folder, the one containing `SKILL.md`, not the
   `.md` file on its own.
4. Describe the task. Claude picks up the matching skill on its own.

In Claude Code, a skill folder goes in `.claude/skills/`.

If the interface has moved, Anthropic's current documentation is at
[support.claude.com](https://support.claude.com) under *Skills*. Availability differs by
plan, and some capabilities have to be switched on before the Skills panel appears.

## The other 15

These 5 come from a set of 20 for running a one-person business, including an offer
builder, an SEO content brief, a landing page audit and a weekly review.

- **[See all 20, with where each one breaks](https://thegentlehours.com/claude-skills)**, no sign-up.
- **[Get all 20 as a download](https://thegentlehours.com/tools)**, free by email, along with a spreadsheet
  of 100 free AI tools that says where each one breaks.

## What these are not

Original workflow instructions written by [The Gentle Hours](https://thegentlehours.com/claude-skills), not
Anthropic's official skills. They give Claude a procedure, not information it does not
have, and they cannot see your accounts or analytics unless you paste them in.

Corrections are welcome: open an issue if a skill misfires.
