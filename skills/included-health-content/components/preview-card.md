# Preview card (provider / clinic)

Rich summary of a provider or option while browsing. Supports an action CTA and a navigation CTA together. Not for a single direct decision with no browsing.

This component **locks** some CTA strings. Those strings win over the glossary preference for `book` on buttons.

## Name / title

- Complete first and last name plus credential
- Do not truncate; wrap as needed

Do: `Dr. Esmeralda Ramirez` / `Jennifer Mouseketeer, NP` / `John Smith, MD`  
Don’t: `Dr. Ramirez` / truncated last names

## AI summary

AI-generated bio summary. Keep it member-facing, specific, and non-clinical-hype. Do not invent specialties or outcomes. (Source spec for this field was incomplete.)

## Locked CTAs

Use sentence case. Visible labels:

| Variant | Primary | Secondary / tertiary |
| --- | --- | --- |
| External provider | `Schedule appointment` | `View full profile` |
| Clinic | `Schedule appointment` | `View more details` |
| IH provider | Time slots replace primary | `View full profile and availability` |

## Time slots (IH providers)

**Time**

- Top of the hour includes `:00`
- No leading zeros
- `AM` / `PM` with no periods, space before the meridian

**Date**

- Abbreviate weekday and month (3 letters, no periods)
- Comma between weekday and month
- No ordinal suffixes
- `Today` instead of the weekday for same-day slots
- `Tomorrow` instead of the weekday for next-day slots

Do: `10:30 AM` + `Thu, Aug 20` / `5:00 PM` + `Today` / `12:15 PM` + `Tomorrow`

## Assistive technology

Include the provider or clinic name in accessible names.

- Save: `Save provider, [name]` / `Remove saved provider, [name]`
- Primary: `Schedule appointment with Dr. Julianna Smith`
- Secondary: `See full profile for Dr. Julianna Smith` (source uses “See” here for the accessible name; visible label stays `View full profile`)
