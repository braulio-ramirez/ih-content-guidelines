# Follow-ups (not v1)

Track later work here so it doesn’t live only in a chat. Each item: why it came up, what to do, what’s blocking.

## Missing source docs

Need PDFs or design-system pages.

| Item | Why | What’s needed |
| --- | --- | --- |
| Inclusive Language Guide | Accessible Writing points to it | PDF or markdown from content |
| Forms guidelines | Form rules now in `components/forms.md`, taken from the Product Content Style Guide Google Doc. Text fields point to them. | Confirm against the PDF or Content Wiki page when available |
| Other pattern pages | UX Copy PDF points to design-system component pages | Those pages, copy specs only |
| Empty states and generic error screens | No component PDFs; v1 uses global UX rules | Component copy PDFs |

## Guideline freshness

| Item | Why | What’s needed |
| --- | --- | --- |
| Updated global and component PDFs | v1 is not the latest brand export | Attach new PDFs and patch the matching markdown (don’t rebuild the whole skill unless structure changed) |
| Get Care catalog | PDF OCR was garbled in places; v1 used cleaner sticker/reference titles | Confirm against a clean source |
| Status glossary | Status Card says never invent a status; v1 uses sticker-sheet values | Official status list if one exists |
| Checkbox vs radio wording | Checkbox content table sometimes said “radio” | Content team confirm if anything still looks wrong |

## Skill behavior and distribution

| Item | Why | What’s needed |
| --- | --- | --- |
| Auto-apply too noisy | Personal install makes the skill available everywhere; auto-apply may fire outside IH work | Set `disable-model-invocation: true` in `SKILL.md` and tell designers to invoke by name (see README) |
| Windows / mixed-OS install | Design team may not all be on macOS | Document and test `%USERPROFILE%\.cursor\skills\` |
| Copy into product repos | Engineers who never personal-install still need guidelines | Copy this package into `app/.cursor/skills/included-health-content/` when a product team wants that |
| Reading-level script | Hemingway-style check was in the old best-practices PDF | Optional script; explicitly out of v1 |

## Healthcare and safety (watch in use)

| Item | Why | What’s needed |
| --- | --- | --- |
| Invented clinical / coverage / price claims | Get Care stickers show costs that may be plan-specific | Tighten SKILL.md if the agent still hallucinates facts |
| Real member PII in examples | Healthcare context | Keep examples generic |
