# Included Health content skill

Cursor skill for drafting and reviewing **Included Health** member-facing UX copy (voice, glossary, component specs).

Source vintage: v1, encoded from Content Style Guideline exports. Later updates patch the markdown in this repo. Designers who cloned the skill pick up changes with `git pull`.

Deferred work: [FOLLOWUPS.md](FOLLOWUPS.md).

## Install (design team)

Clone this repo once as a **personal skill**. Cursor can then use it in every project on your machine.

**macOS / Linux**

```bash
git clone <internal-repo-url> ~/.cursor/skills/included-health-content
```

**Windows** (see also [FOLLOWUPS.md](FOLLOWUPS.md))

```bash
git clone <internal-repo-url> %USERPROFILE%\.cursor\skills\included-health-content
```

Do not put this folder in `~/.cursor/skills-cursor/` (Cursor’s built-in skills).

### Update

```bash
cd ~/.cursor/skills/included-health-content && git pull
```

### Optional: product repos

To ship the guidelines with a product codebase (everyone who clones that app gets them), copy this repo’s files into:

`your-app/.cursor/skills/included-health-content/`

Content/UX owns this repo. Don’t fork copies to edit in ten places.

## Available vs auto-apply

Installing the skill and using the skill are different:

| | Meaning |
| --- | --- |
| **Personal install** | The skill is *available* in every Cursor project on that machine. |
| **Auto-apply (v1 default)** | The agent *may load it without being asked* when the chat looks like Included Health product/member copy. |
| **Explicit only** | The skill stays installed but runs only when you name it. |

v1 **omits** `disable-model-invocation` in `SKILL.md`, so auto-apply is on. The skill description is scoped to Included Health so it should not restyle unrelated work (for example a random “write a button label” in a non-IH project).

If auto-load is too noisy:

1. In `SKILL.md`, add this line to the YAML frontmatter (with the other fields):

   `disable-model-invocation: true`

2. Invoke it by name, for example: “Use the Included Health content skill” or “Review this copy against IH content style.”

That change is also listed in [FOLLOWUPS.md](FOLLOWUPS.md) if we want to make explicit-only the default later.

## How to use it

- Ask for new product copy (empty states, CTAs, form labels, cards, calendars).
- Paste existing copy and ask for a review against Included Health guidelines.
- Mention Included Health, member-app copy, or this skill if the agent doesn’t pick it up.
