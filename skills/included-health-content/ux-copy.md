# UX copy, page structure, and accessible writing

Aim for a 7th–8th grade reading level. Keep copy concise enough to fit on a mobile screen without scrolling when possible; don’t cut so far that the message loses value. Use whitespace. Stay consistent with the UX/UI glossary.

Empty states and generic full-page errors have no component spec yet. Use this file plus [voice.md](voice.md).

## Text elements

| Element | POV | Case | Punctuation | Word count | Other |
| --- | --- | --- | --- | --- | --- |
| Screen titles (title in the top secondary navigation bar) | Neutral | Title Case | Always omit | 1–3 words | The only header exception to sentence case. |
| Headers | Second person (`you` / `your`) or neutral | Sentence case, except screen titles (see Screen titles row) | Always omit (unless a question) | 3–7 words; should not exceed two lines | |
| Body copy | Second person or neutral | Sentence case | Always include | No official limit; stay concise | Break bulky paragraphs into lists |
| CTAs | Neutral (exception: “Contact us”) | Sentence case | Always omit | 1–4 words | Lead with the user’s objective. Be clear about the action. Match language in header/body. Prefer short words (`book` not `schedule`, `visit` not `appointment`) unless a component spec locks a different string. |
| Lists | Second person or neutral | Sentence case | If one item is a full sentence with punctuation, all items get punctuation; otherwise omit | No official limit; stay concise | Bullets when order doesn’t matter; numbers when sequence matters. Parallel structure (if one item starts with a verb, they all do). |

## Language and page structure

**Clear, concise, consistent**

- Do not use “read more” or “click here.” Write specific link and button labels so users know what happens next.
- Do not reuse the same hyperlink text on one page for different destinations.
- Use the same terminology for the same action throughout the product.
- Keep sentences short. Avoid adjectives and adverbs when possible. Prefer shorter words over multi-syllable ones.

**Scannable**

- Chunk copy into logical blocks.
- Use whitespace between blocks.
- Use heading tags (H1, H2, H3) for hierarchy.

**No visual-only cues**

- Avoid directional language (`left`, `right`, `above`, `below`). Screen readers don’t have that map, and layout shifts on mobile.
- Do not describe elements only by color.
- Prefer `select` over gestural terms (clicking, tapping, pressing).

**Alt text**

- Describe what the image communicates. No keyword stuffing.
- Do not describe gender, age, or race unless it is required to understand the content.
- Do not start with “image of” — it is implied.
- Decorative images: empty alt (screen readers skip them).
- Videos: captions and transcriptions.

## Money

Medical costs and coverage are a major topic in member copy. Source: Product Content Style Guide, Money section.

- Omit cents on whole-dollar amounts: `$10`, not `$10.00`.
- Always use a comma to separate thousands: `$2,000`, not `$2000`.
- Write the exact amount. Never round: `$525.78`, not `$526`.

## Punctuation in UI copy

- Do not use an asterisk as a footnote marker. Use a tooltip for extra information. Asterisks mark required form fields only (see [forms.md](components/forms.md)).
- Do not use ellipses in CTAs.

## Error messages

Applies to error copy that has no component spec. Component specs (text fields, banners) add their own rules. Source: Product Content Style Guide (Google Doc), Error Messages section.

**Tone**

- Be humble. Never blame the member. Use passive voice when active would place blame (see [voice.md](voice.md)): `Incorrect password entered.`, not `You entered an incorrect password.`
- Use clear language and avoid ambiguity. Keep messages short, concise, and meaningful.
- Always give a next step. Do not leave the member hanging.
- Avoid unnecessary, overly negative words.
- Avoid technical jargon.
- Do not use all caps. It can feel like yelling.

**Error types**

| Type | Use for | Component | Rules that apply |
| --- | --- | --- | --- |
| Field validation | Errors within a form field | Text field error | [text-fields.md](components/text-fields.md), [forms.md](components/forms.md) |
| Screen-level error banner | Errors that apply to an entire screen or section | Page banner | [banners.md](components/banners.md), page banner |
| Inline error banner | Errors that apply to one section of the screen | Inline banner | [banners.md](components/banners.md), inline banner |
| Error screen | General technical errors | Full-page error | Tone rules in this section. A full-page error is not a banner. No wording or length spec yet. |

## Accessible writing

Accessible content also helps people on small screens, older people, temporary disabilities (broken arm, lost glasses), situational limits (bright sun, no audio), and slow or expensive connections.

- Prioritize simplicity and perceivability. Familiar, consistent interactions. Everyone should be able to perceive content (sight, hearing, or touch).
- People-first when writing about disability. Accomplishments and goals before a disability when relevant. Use the language a specific person or community uses for themselves (see [inclusive-language.md](inclusive-language.md)).
- Avoid language that uses a disability to express a negative quality.
