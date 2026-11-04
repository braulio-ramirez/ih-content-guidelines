---
name: included-health-content
description: >-
  Drafts and reviews member-facing UX copy against Included Health Content Style
  Guidelines (voice, glossary, buttons, text fields, checkboxes, radios,
  dropdowns, lists, calendars, status/preview/get-care cards, page banners,
  inline banners, toasts, CTAs, microcopy).
  Use when the user is writing or reviewing Included Health product or member-app
  copy, mentions Included Health / IH content style, or asks to apply this skill.
  For a structured review of existing copy, prefer the review-content skill.
  Do not use for generic coding, non-IH products, or copy not tied to Included Health.
---

# Included Health content style

Source vintage: v1 encoded from Content Style Guideline exports provided for this skill. Later PDF updates overwrite these markdown files. See [FOLLOWUPS.md](../../FOLLOWUPS.md).

Apply these guidelines to **in-product / UX content** (titles, headers, body, CTAs, lists, empty states, errors, forms, cards). If the surface might be marketing or email, ask before treating it as product UX — the source docs are UX-first.

Do not invent clinical claims, coverage, wait times, or prices. Get Care stickers may show plan-specific cost. Do not use real member PII in examples.

Out of scope until added: Inclusive Language Guide, Forms guidelines. Empty states and generic errors use global UX rules in [ux-copy.md](ux-copy.md).

## Precedence

When sources disagree, the more specific file wins:

1. Matching file(s) in `components/`
2. [terminology.md](terminology.md)
3. [ux-copy.md](ux-copy.md)
4. [voice.md](voice.md)

Example: glossary prefers `book` on CTAs; Preview Card locks **Schedule appointment** — use the Preview Card string on that component.

## Write workflow

1. Confirm the work is Included Health member/product copy.
2. Identify the surface and component(s).
3. Read the matching `components/` file(s). If a screen includes buttons, time slots, or other nested elements, also read those files (parent + [components/buttons.md](components/buttons.md) and/or [components/calendar.md](components/calendar.md) as needed).
4. Apply voice and glossary ([voice.md](voice.md), [terminology.md](terminology.md), [ux-copy.md](ux-copy.md) as needed).
5. Draft at a 7th–8th grade reading level. Prefer short, scannable copy.
6. Accessibility pass: no directional or color-only language; descriptive links/buttons; `select` not `click`/`tap`; people-first disability language.

**Draft output:** copy keyed by UI element (for example Label, Help text, CTA) so it can be pasted into Figma. Note any guideline you could not apply because facts were missing.

## Review workflow

For a full structured review (issues table with cited rules + revised copy), use the `review-content` skill. Quick inline checks can follow these steps:

1. Identify component(s) and read those specs first.
2. Check the global non-negotiables and glossary.
3. List violations (quote the copy + the rule).
4. Provide a rewritten version.

See [examples.md](examples.md) for before/after pairs.

## Component router

Read only the files that apply:

| If the work is… | Read |
| --- | --- |
| Buttons / CTAs / action labels | [components/buttons.md](components/buttons.md) |
| Text field / input / placeholder / help / field error | [components/text-fields.md](components/text-fields.md) |
| Checkbox (multi-select) | [components/checkboxes.md](components/checkboxes.md) |
| Radio (single-select) | [components/radio-buttons.md](components/radio-buttons.md) |
| Dropdown / select / picker | [components/dropdowns.md](components/dropdowns.md) |
| List / list item | [components/lists.md](components/lists.md) |
| Calendar / date / time slot | [components/calendar.md](components/calendar.md) |
| Status card / request status / wait time | [components/status-card.md](components/status-card.md) |
| Preview / provider / clinic card | [components/preview-card.md](components/preview-card.md) |
| Get care tile / service grid | [components/get-care-card.md](components/get-care-card.md) |
| Action Center card / task card / event card / New tag | [components/action-center-card.md](components/action-center-card.md) |
| Page banner / inline banner / toast | [components/banners.md](components/banners.md) |

## Non-negotiables

- Conversational, not clinical. Contractions are OK. No slang, emojis, unexplained acronyms, misspellings, or texting language.
- No exclamation points for emphasis.
- Do not assume gender or pronouns from a name, voice, or appearance. Default to gender-neutral words (`spouse`, `child`, `person`). Use gender-affirming pronouns when that information is available.
- Do not use “Included” out of context (for example “On-call care on your phone—Included.”).
- Do not appropriate words from other languages and cultures (`voila`, `pronto`, `pow wow`).
- Do not assume familiarity or how the member feels. Do not exaggerate casual tone (“How ya doin?”).
- No cliches, jokes, corporate buzzwords, or predictable marketing hooks (“New Year, New You.”).
- Prefer `select` over `click` or `tap`; `tap` is allowed in push notification copy only; `scroll` over `swipe`; `turn on` / `turn off` over `toggle`.
- Speak to the member in second person when the UX table allows it. Use consistent glossary terms.

## Additional resources

- Voice, personality, and tone: [voice.md](voice.md)
- UX elements, page structure, accessible writing: [ux-copy.md](ux-copy.md)
- Glossary: [terminology.md](terminology.md)
- Before/after examples: [examples.md](examples.md)
