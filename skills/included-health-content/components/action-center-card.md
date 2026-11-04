# Action Center card

Cards in the Action Center: **task cards** (something the member needs to do) and **event cards** (a video or phone visit with an Included Health provider). Source: Figma, IH Design System, Anatomy → Content Spec: Elements (Table).

Shared rules for every text element on both card types come first. Then the element-specific rules.

## Shared rules (all text on task and event cards)

- Sentence case
- No end punctuation
- Plain language at a 7th–8th grade reading level
- Text never truncates, so character counts are targets for scannability, not hard caps
- A tag’s meaning must be in its words, not only its color
- Times: `A.M.` and `P.M.`, all caps with periods
- Months: abbreviated, no period

Do: `Mon, Nov 16, 8:30 A.M.` / `Due Nov 16`  
Don’t: `8:30 AM` / `8:30 a.m.` / `Due Nov. 16.`

## New tag

Signals that a card was just added to the Action Center.

- Text is always `New`
- Green, center aligned with other tags, always first
- Appears when a card is newly added to the Action Center
- Disappears when the member selects the card or 24 hours after it’s added, whichever comes first
- Doesn’t count toward the 2-tag limit on task cards

Do: `New` + `Mon, Nov 16, 8:30 A.M.` (event card) / `New` + `Due in 3 days` (task card)  
Don’t: `New!` / `Just added`

## Task card

### Title

- Instead of a button, the Title is the main call to action. The whole card is tappable.
- Start with a verb, then “your” and the thing
- About 34 characters (1 line)
- Name the action the card opens, so the Title matches the next screen

Do: `Pay your $10 bill` / `Update your coverage on file` / `Schedule your colonoscopy`  
Don’t: `Coverage update needed` (no verb) / `Bill payment` (no action)

### Description

The most useful context for the Title: why it matters or what happens next.

- About 40 characters (1 line), 75 max (2 lines)
- Don’t repeat the Title
- Add the year only if it isn’t the current year

Do: `For accurate benefits and pricing` / `For your visit on Aug 25, 2025` / `Pick up where you left off` (abandoned visit cart)  
Don’t: `Pay this bill now` (repeats the Title) / `Secure your preferred date and time before it’s gone` (pressure tactic)

### Tags

Status, timing, and effort, so members can decide what to do first.

- `New` (if applicable)
- Order: status, then timing or effort
- Allowed: `Overdue`, `Due tomorrow`, `Due in [n] days`, `Due [Mon D]`, `Takes [n] min`, `Referred [n] days ago`
- Don’t repeat info from the Title or Description
- Don’t pair 2 tags that say the same thing

Do: `Overdue` + `Takes 5 min` (urgency plus low effort) / `Due in 3 days` / `Referred 4 days ago`  
Don’t: `Overdue` + `Due on Sept 1` (same fact twice)

### Overflow menu

- Accessible name: `More options`
- Menu items start with a verb
- Sentence case, no end punctuation

Do: `More options` (accessible name)  
Don’t: `Menu` or `…` (accessible name)

## Event card (video or phone visit with an Included Health provider)

### Title

What the visit is and who it’s for.

- More than 5 min before start: `[Video/Phone] visit for [first name]`
- Use the first name for account holders and dependents alike
- Video visits, from 5 min before start (when members can join): `Join video visit for [first name]`
- Phone visits don’t change, because the provider calls the member
- About 24 characters when the avatar shows; longer names wrap to 2 lines

Do: `Video visit for Riley` / `Join video visit for Riley` (5 min before start) / `Phone visit for Emma`  
Don’t: `Your video visit` / `Join your video visit` / `Phone consult for Emma`

### Description

Who the visit is with.

- Provider’s full name and credential
- Required whenever the avatar shows
- If no provider is assigned yet (for example, urgent care), use `First available provider`

Do: `Jane Smith, MD` / `Alex Lee, NP` / `First available provider`  
Don’t: `Dr. Jane Smith, MD` (Dr. and MD say the same thing)

### Time tag

When the visit is, or the expected wait for on-demand urgent care.

- Scheduled visits: always the visit’s date and time
- Today or tomorrow: `Today, H:MM A.M./P.M.` or `Tomorrow, H:MM A.M./P.M.`
- Any other day: `Day, Mon D, H:MM A.M./P.M.`
- Add the year only if it isn’t the current year
- No countdowns or status words (`Starts in`, `Happening now`)
- On-demand urgent care: `Estimated wait: [n] min`

Do: `Today, 2:30 P.M.` / `Tomorrow, 8:30 A.M.` / `Mon, Nov 16, 8:30 A.M.` / `Estimated wait: 12 min` (on-demand urgent care)  
Don’t: `Tomorrow 8:30 AM` (missing comma, wrong A.M. style) / `Starts in 5 min` / `Happening now`

### Quick action

Lets members save the visit to their calendar.

- Accessible name: `Add to calendar`
- Consider hiding it once the Title switches to `Join`

Do: `Add to calendar` (accessible name)  
Don’t: `Calendar` (doesn’t describe the action)
