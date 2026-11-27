# skill-granteln

An [Agent Skill](https://agentskills.io) that makes your coding agent talk like
a Bavarian **Grantler**, a dry, grumpy, fundamentally helpful grumbler from
Upper or Lower Bavaria. It covers the dialect (Mittelbairisch, with
Ober- and Niederbayern variants) and the mentality behind it. The agent still
does the work properly, and code and commands stay in standard language.

## Install

Clone or copy this folder (it must keep the name `skill-granteln`) into your
agent's skills directory:

| Agent | Global path | Project path |
|---|---|---|
| Claude Code | `~/.claude/skills/skill-granteln/` | `.claude/skills/skill-granteln/` |
| Cursor | `~/.cursor/skills/skill-granteln/` | `.cursor/skills/skill-granteln/` |
| Codex, Gemini CLI, Amp and other agents that read `.agents` | `~/.agents/skills/skill-granteln/` | `.agents/skills/skill-granteln/` |

Some versions of Codex and Gemini CLI use `~/.codex/skills/` or
`~/.gemini/skills/` instead. If yours doesn't pick up the skill, check its
documentation for the right path.

```bash
git clone <this-repo> ~/.claude/skills/skill-granteln
```

For agents without skill support, paste the contents of `SKILL.md` into their
system prompt or `AGENTS.md`.

## Always on

Agents load skills based on the `description`. This one asks to be used for
every reply and offers itself when you get impatient or start swearing. To
force it on, add a line like this to your `CLAUDE.md` or `AGENTS.md`:

```
Always use the skill-granteln skill.
```

## Files

- `SKILL.md`: mentality, dialect, phrases, intensity levels and behaviour rules
- `references/glossary.md`: extended vocabulary, loaded on demand
