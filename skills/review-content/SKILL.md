---
name: review-content
description: >-
  Reviews a piece of Included Health member-facing UX copy against the Included
  Health Content Style Guidelines and returns each issue with the rule it breaks,
  plus a rewritten version. Use when the user pastes or points to existing IH
  product or member-app copy (a screen, component, CTA, banner, card, form field,
  error, empty state) and asks to review, critique, check, audit, or improve it.
  Do not use for drafting new copy from scratch (use included-health-content),
  for non-IH products, or for code review.
argument-hint: "[copy to review, or a description of where it lives]"
---

# Review Included Health copy

This skill reviews copy. The guidelines themselves live in the sibling skill folder `../included-health-content/`. Read rules from there; do not restate or invent rules here. If a rule isn't in those files, it isn't a rule — at most it's a suggestion, and it must be labeled as one.

Guideline files (paths relative to this skill's folder):

- Overview, non-negotiables, precedence, component router: [../included-health-content/SKILL.md](../included-health-content/SKILL.md)
- Voice, personality, tone: [../included-health-content/voice.md](../included-health-content/voice.md)
- UX elements, page structure, accessible writing: [../included-health-content/ux-copy.md](../included-health-content/ux-copy.md)
- Glossary: [../included-health-content/terminology.md](../included-health-content/terminology.md)
- Before/after pairs: [../included-health-content/examples.md](../included-health-content/examples.md)
- Component specs: `../included-health-content/components/`

## Workflow

1. **Get the copy.** Use what the user pasted (or `$ARGUMENTS`). If there's no copy, ask for it. If it's unclear whether this is in-product UX or marketing/email, ask — the guidelines are UX-first.
2. **Load the rules.** Always read `../included-health-content/SKILL.md` (non-negotiables, precedence) and `terminology.md`. Use its component router table to pick the matching `components/` file(s); also read `buttons.md` if the copy has CTAs and `calendar.md` if it has dates or time slots. Read `voice.md` and `ux-copy.md` for tone, structure, and accessibility.
3. **Identify each UI element** (title, body, CTA, label, help text, error, banner, and so on). If the user didn't say which component it is, infer it and state your assumption.
4. **Check every element** against, in this order:
   - Component spec (character limits, required parts, locked strings)
   - Non-negotiables
   - Glossary terms
   - UX copy and accessibility rules (no directional or color-only language, descriptive links and buttons, `select` not `click`/`tap`, people-first language)
   - Voice and tone, 7th–8th grade reading level
   When rules conflict, follow the precedence order in `../included-health-content/SKILL.md` (the more specific file wins).
5. **Rewrite** only what needs to change. Keep the meaning. Don't invent clinical claims, coverage, wait times, prices, or other facts — if a fix needs a fact you don't have, leave a placeholder like `[wait time]` and list it under Questions.

## Output

Use this structure, in this order. Keep it short and pasteable into Figma comments.

**Verdict:** one line — `Ready to ship`, `Minor fixes`, or `Needs rework` — plus the single most important fix.

**Issues**

| # | Element | Current copy | Issue | Rule (file) | Suggested fix |
| --- | --- | --- | --- | --- | --- |
| 1 | CTA | "Click here to book!" | Gesture word, exclamation point, vague link | Non-negotiables (SKILL.md); Buttons (components/buttons.md) | "Book visit" |

- Quote the copy exactly.
- Cite the file the rule comes from so the designer can check it.
- Order by severity: component-spec and non-negotiable breaks first, then glossary, then accessibility, then tone polish.
- Mark anything that's taste rather than a written rule as **Suggestion**.

**Revised copy** — keyed by UI element so it can be pasted straight in:

```
Title: …
Body: …
Primary CTA: …
```

**Questions** — only if facts were missing or a rule couldn't be applied. Omit this section otherwise.

If there are no issues, say so, and skip the table and the revised copy.
