# Included Health content skill

Claude Code plugin and Cursor skills for drafting and reviewing **Included Health** member-facing UX copy (voice, glossary, component specs).

Source vintage: v1, encoded from Content Style Guideline exports. Later updates patch the markdown in this repo. Claude Code installs pick up changes automatically; Cursor installs use `git pull`.

Deferred work: [FOLLOWUPS.md](FOLLOWUPS.md).

## What's in here

| Skill | What it does |
| --- | --- |
| `included-health-content` | Drafts new copy and does quick checks. Holds all the guidelines. |
| `review-content` | Reviews existing copy: issues table with the rule each one breaks, plus revised copy. Reads the same guideline files — no second copy to maintain. |

**Edit guidelines in `skills/included-health-content/`.** Both skills pick up the change.

## Install in Claude Code (auto-updates)

This repo is a Claude Code plugin and its own marketplace. Run once in a terminal:

```bash
claude plugin marketplace add braulio-ramirez/ih-content-guidelines
claude plugin install ih-content-guidelines@ih-content
```

Then turn on auto-update (one time): run `claude`, type `/plugin`, go to **Marketplaces**, select `ih-content`, and select **Enable auto-update**.

After that, every push to `main` reaches you the next time you start a session. To update by hand:

```bash
claude plugin update ih-content-guidelines@ih-content
```

Use it by asking for IH copy help, or by name: `/ih-content-guidelines:review-content <paste copy>`.

**Private repo?** Background updates use the git login already on your machine and never prompt. Run `gh auth login`, then `gh auth setup-git`, once.

**For maintainers:** don't add a `version` field to `.claude-plugin/plugin.json` or `marketplace.json`. Without it, installs follow commits. With it, nobody gets changes until the version string changes. Check edits with `claude plugin validate .`.

## Install in Cursor

The skills now live under `skills/`. Clone the repo anywhere, then link each skill into Cursor's personal skills folder.

**macOS / Linux**

```bash
git clone <internal-repo-url> ~/ih-content-guidelines
ln -s ~/ih-content-guidelines/skills/included-health-content ~/.cursor/skills/included-health-content
ln -s ~/ih-content-guidelines/skills/review-content ~/.cursor/skills/review-content
```

**Already installed the old way?** The old layout cloned the repo straight into `~/.cursor/skills/included-health-content`. After this change that folder no longer has `SKILL.md` at its top level, so remove it and use the steps above:

```bash
rm -rf ~/.cursor/skills/included-health-content
```

Windows: see [FOLLOWUPS.md](FOLLOWUPS.md).

Do not put these folders in `~/.cursor/skills-cursor/` (Cursor's built-in skills).

### Update (Cursor)

```bash
cd ~/ih-content-guidelines && git pull
```

### Optional: product repos

To ship the guidelines with a product codebase, copy `skills/included-health-content/` and `skills/review-content/` into `your-app/.cursor/skills/` (keep them side by side — `review-content` reads the guideline files from its sibling folder).

Content/UX owns this repo. Don't fork copies to edit in ten places.

## Available vs auto-apply

Installing the skill and using the skill are different:

| | Meaning |
| --- | --- |
| **Personal install** | The skill is *available* in every Cursor project on that machine. |
| **Auto-apply (v1 default)** | The agent *may load it without being asked* when the chat looks like Included Health product/member copy. |
| **Explicit only** | The skill stays installed but runs only when you name it. |

v1 **omits** `disable-model-invocation` in `SKILL.md`, so auto-apply is on. The skill description is scoped to Included Health so it should not restyle unrelated work (for example a random “write a button label” in a non-IH project).

If auto-load is too noisy:

1. In `skills/included-health-content/SKILL.md`, add this line to the YAML frontmatter (with the other fields):

   `disable-model-invocation: true`

2. Invoke it by name, for example: “Use the Included Health content skill” or “Review this copy against IH content style.”

That change is also listed in [FOLLOWUPS.md](FOLLOWUPS.md) if we want to make explicit-only the default later.

## How to use it

- Ask for new product copy (empty states, CTAs, form labels, cards, calendars).
- Paste existing copy and ask for a review against Included Health guidelines.
- Mention Included Health, member-app copy, or this skill if the agent doesn’t pick it up.
