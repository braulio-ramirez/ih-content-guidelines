# Banners

Page banners, inline banners, and toasts. Pick the component before writing the words.

Action labels follow [buttons.md](buttons.md) for sentence case, no punctuation, and glossary verbs (`book`, `visit`). Length caps in this file win over the buttons spec’s 4-word allowance.

The dismiss control is an **X**. Its accessible name is **Dismiss notification**.

## Which component

- **Toast:** the member just did something, and the system is closing the loop (confirmed, failed, or still in progress). A message that needs more than a retry is a modal, not a toast.
- **Page banner:** the system has something to say that the member did not trigger, and it covers the whole page or a service state. One per page, at the top of the content, below the nav.
- **Inline banner:** the system has something to say that the member did not trigger, and it covers one section of content. Place it next to that content. More than one on a page is fine when each points at different content.

Do not use these for promotional or feature-awareness messages. A full-page error (only when there is no page to go back to) is not a banner.

Error banners follow the rules for their type. An error that applies to the whole screen or a section of the screen uses the page banner rules (screen-level error banner). An error that applies to one section uses the inline banner rules (inline error banner). Field-level errors are not banners; see [text-fields.md](text-fields.md) and [forms.md](forms.md). Error copy tone rules are in [ux-copy.md](../ux-copy.md).

## Page banner

Dismiss only advisory messages. An ongoing condition the member cannot ignore stays on the page.

### Elements

These rules apply to every page banner, including the examples below.

#### Title

- **Role:** clearly alerts the member to a service status, time-bound availability, a usage limit, an account prompt, or a page load failure.
- **Copy guidelines:** 3–5 words (7 max). No punctuation. Not a question. Lead with the status the member cares about, not “We” or “Our system.” Use the passive-voice exception when it avoids placing blame.

Do: `Messaging temporarily offline` / `Chat limit reached`  
Don’t: `We are experiencing a messaging outage` / `You reached your chat limit`

#### Body

- **Role:** says what is still possible or what happens next.
- **Copy guidelines:** 2 sentences at most, and only when it adds something the title does not. Cut filler.

Do: `You can still book appointments. Messaging returns by 9am ET.`  
Don’t: `Our team is investigating.`

#### Action line

- **Role:** the best next step, if there is one.
- **Copy guidelines:** 1–3 words. A destination verb plus an object. A text link, not a filled button.

Do: `Book visit`  
Don’t: `Click here` / `Learn more`

### Common examples

Each example adds tone. It still follows the element rules above.

- **Service status.**
  - **Role:** clarifies a system state the member did not cause.
  - **Tone:** neutral and factual. No apology filler. Include a workaround when there is one.
  - Do: `Messaging is offline. You can still book appointments in Get Care.`
- **Usage limit.**
  - **Role:** alerts the member about a cap they hit.
  - **Tone:** a neutral fact, not a rule violation, plus a workaround. The title follows the title rule above (`Chat limit reached`). Put the workaround in the body.
  - Do: title `Chat limit reached`, body `Try calling us.`
  - Don’t: `You reached today's chat limit` / `You exceeded your limit.`
- **Time-bound availability.**
  - **Role:** calls out hours or a time window.
  - **Tone:** concrete. Do not use “soon” or “later.”
  - Do: `Enrollment closes Nov 1`
  - Don’t: `Enrollment closes soon`
- **Account prompt.**
  - **Role:** prompts an account or settings action.
  - **Tone:** state the value and the main action.
  - Do: `Add to your calendar`
- **Load failure.**
  - **Role:** a system error.
  - **Tone:** honest and retry-oriented.
  - Do: `This page didn't load. Select retry.`

## Inline banner

Tie each banner to one area of content. Do not stack banners on top of each other.

Dismiss tips and optional guidance only. Do not allow dismiss for fees, compliance disclosures, or anything the member must see.

A validation message on a text field follows [text-fields.md](text-fields.md). The validation example below is for a banner next to a section.

### Elements

These rules apply to every inline banner, including the examples below.

#### Title

- **Role:** states what the banner is about (a fee, a disclosure, and so on).
- **Copy guidelines:** one clear line, 3–5 words (7 max). No punctuation. The specific fact does not go in the title.

Do: `Late cancellation fee`  
Don’t: `A fee applies if you cancel less than 24 hours in advance`

#### Body

- **Role:** gives the specific, actionable detail (amount, date, or condition).
- **Copy guidelines:** 1 sentence ideal, 2 max. Exact, never vague, and not a repeat of the title.

Do: `A $100 fee applies if you cancel within 24 hours.`  
Don’t: `A fee may apply if you're late.`

#### Action line

- **Role:** the best next step, if there is one.
- **Copy guidelines:** 1–3 words, and only when the member can act. Omit it when there is nothing to do. `Got it` is dismiss, not the action.

### Common examples

Each example adds tone. It still follows the element rules above.

- **Fee or cost notice.**
  - **Role:** clarifies the type of fee or cost.
  - **Tone:** neutral and factual, with the exact amount.
  - Do: `A $50 fee applies if you miss your appointment.`
  - Don’t: `A fee may apply if you miss your appointment.`
- **Compliance disclosure.**
  - **Role:** adds legally or clinically required information.
  - **Tone:** plain language, neutral and factual.
  - Do: `This plan does not cover out-of-network providers.`
- **Clinical guidance.**
  - **Role:** explains an unfamiliar clinical term or concept.
  - **Tone:** name the term, then define it in plain language.
  - Do: `A biosimilar is a lower-cost medicine that works the same way as your current one.`
- **Validation error.**
  - **Role:** states the wrong format.
  - **Tone:** the body says what is wrong and shows the expected format.
  - Do: `Enter a valid phone number, like 555-123-4567.`
- **Tip.**
  - **Role:** optional, skippable guidance.
  - **Tone:** lead with the value. Lighter, and specific enough to be useful.
  - Do: title `Save time next visit`, body `Favorite this provider to book faster next time.`

## Toast

Copy must stand on its own. The member may not see what triggered it. Never truncate.

In-progress copy must change to a distinct completion string. It does not disappear without a new message.

### Elements

These rules apply to every toast, including the examples below.

#### Title

- **Role:** confirms the outcome, expected or unexpected, of what the member just did.
- **Copy guidelines:** one clear line, 3–5 words (7 max). No punctuation. Name the object or action.

Do: `Member ID copied`  
Don’t: `Copied`

#### Body

- **Role:** adds detail only when the title alone is not enough.
- **Copy guidelines:** optional. Most toasts do not need one. Add it only for a next step or a clarifying detail.

Do: title `Message sent`, body `Expect a reply within 24 business hours.`

#### Action line

- **Role:** the best next step, if one is available.
- **Copy guidelines:** 1 word ideal, 2 max. A single known action, not a general CTA.

Do: `Undo`  
Don’t: `Undo this action`

### Common examples

Each example adds tone. It still follows the element rules above.

- **Confirmation.**
  - **Role:** states that the action was completed.
  - **Tone:** past tense. A plain statement of what happened.
  - Do: `Feedback sent`
  - Don’t: `You successfully submitted your feedback`
- **Failure.**
  - **Role:** states that the action was not completed.
  - **Tone:** say what failed and, when it helps, why or what to do. Avoid a vague “Something went wrong” when the cause is known.
  - Do: `Message didn't send. Check your connection and try again.`
  - Don’t: `Error occurred`
- **In progress.**
  - **Role:** clarifies that the action is still underway.
  - **Tone:** present progressive (`-ing`). The completion message is a new string.
  - Do: `Uploading your document…` then `Upload successful`
