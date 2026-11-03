# UX copy, page structure, and accessible writing

Aim for a 7th–8th grade reading level. Keep copy concise enough to fit on a mobile screen without scrolling when possible; don’t cut so far that the message loses value. Use whitespace. Stay consistent with the UX/UI glossary.

Empty states and generic full-page errors have no component spec yet. Use this file plus [voice.md](voice.md).

## Text elements

| Element | POV | Case | Punctuation | Word count | Other |
| --- | --- | --- | --- | --- | --- |
| Page titles | Neutral | Title Case | Always omit | 1–3 words | |
| Headers | Second person (`you` / `your`) or neutral | Sentence case | Always omit (unless a question) | 3–7 words; should not exceed two lines | |
| Body copy | Second person or neutral | Sentence case | Always include | No official limit; stay concise | Break bulky paragraphs into lists |
| CTAs | Neutral (exception: “Contact us”) | Sentence case | Always omit | 1–3 words | Lead with the user’s objective. Be clear about the action. Match language in header/body. Prefer short words (`book` not `schedule`, `visit` not `appointment`) unless a component spec locks a different string. |
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

## Accessible writing

Accessible content also helps people on small screens, older people, temporary disabilities (broken arm, lost glasses), situational limits (bright sun, no audio), and slow or expensive connections.

- Prioritize simplicity and perceivability. Familiar, consistent interactions. Everyone should be able to perceive content (sight, hearing, or touch).
- People-first when writing about disability. Accomplishments and goals before a disability when relevant. Use the language a specific person or community uses for themselves (Inclusive Language Guide is not in this skill yet).
- Avoid language that uses a disability to express a negative quality.
