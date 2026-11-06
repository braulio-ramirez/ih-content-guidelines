# Common terminology (UX/UI glossary)

Use these terms consistently. Component specs override this file when they lock a string.

## Gestural terms

| Term | Definition | Guidelines |
| --- | --- | --- |
| Click | Mouse-only | Avoid. Use `select`. |
| Scroll | Moving content on screen | Use `scroll` instead of `swipe` (more device-agnostic). |
| Select | Picking an element in the UI | Preferred instead of `click` or `tap`. Do not use `select` for a non-UI decision such as picking a doctor — use `choose`. |
| Swipe | Touchscreen-only | Avoid. Use `scroll`. |
| Tap | Touchscreen-only | Avoid. Use `select`. Exception: push notification copy, where `tap` is allowed (e.g. “Tap to pay.”). |
| Toggle | Enable/disable a control | Don’t say `toggle`. Write `turn on` / `turn off` (e.g. “Turn location services on”). |
| Type | Entering text | In Messages, use `type` to instruct members chatting with Dot or the Care Team. Elsewhere, prefer `enter`. |

## Dual actions

| Pair | Meaning | Use when |
| --- | --- | --- |
| Add / Remove | Show or hide content that already exists in the system | Native product content. Do not use `delete` as a substitute for `remove`. |
| Continue / Cancel | Move forward or exit | Only one way forward; cannot skip or go back. |
| Next / Back | Next or previous step | Multi-step flows where the user goes back and forth. |
| Next / Previous | Next or previous page | Pagination (e.g. search results). |

## Affirmative actions

| Term | Guidelines |
| --- | --- |
| Agree | Consent to high-stakes notices (terms, legal). Do not use `OK` interchangeably here. |
| Enter | Inputting new information (e.g. registration). Preferred over `type` because it is more neutral (except in Messages; see Type). |
| OK | Acknowledgement. Style as **OK** (all caps), not “okay.” Do not use for high-stakes consent. |
| Send | Messages only. Not for forms (`submit`) or sharing with another party (`share`). |
| Share | Sending information to another party (e.g. documents with the Care Team). Not for messaging or forms. |
| Start | Don’t use as a standalone CTA. Use **Get started** on buttons. |
| Submit | Forms and button CTAs. Standalone `Submit` is OK on a button. Not for messages (`send`) or sharing with another party (`share`). |

## Dismissive actions

| Term | Guidelines |
| --- | --- |
| Close | Don’t write the word “close.” Use an **X** icon to close a window or modal. |
| Delete | Permanent erase of something not native to the product (e.g. a document the user uploaded). |
| Dismiss | User does not want to be shown something ever again. Not for acknowledgement or completion (use `OK`). |
| Skip | Multi-step flows only, and only for steps that are not required. |

## General actions

| Term | Guidelines |
| --- | --- |
| Book | Conversational alternative to `schedule` for appointments. Use **book** in CTAs (shorter). |
| Choose | Decision-making (e.g. choosing a doctor). OK in body copy. Avoid in CTAs — use `select` for UI. |
| Schedule | Booking an appointment. Use in descriptive body text; use `book` in CTAs unless a component spec locks another label. |
| Upload | Transfer digital assets from the user’s device to the system (e.g. insurance card photo). |
| View | Access additional information. Don’t use `view` or `view more` as a standalone CTA — say what they will view (e.g. “View more providers”). Prefer `view` over `see`. |

## Feature and service names

Describe what the member gets in plain words. Use an official name only when the member needs it to find or identify the product, and spell it as the Products list does. Source: Product Content Style Guide (Slang and Jargon) and Included Health Terms.

| Avoid in everyday copy | Say instead |
| --- | --- |
| Provider Match | Finding a doctor |
| Expert Medical Opinion | Second opinion |
| Claims Advocacy | Describe the help. Example: "Send us your doctor bill. We'll double check with your insurance and doctor's office if it's correct." |
| Claims History | Care History (capitalize when it names the app section) |
| Cost Transparency | Cost estimate |
| Concierge Referral, Benefits Navigation Directory, Financial Toolkit, "navigation" | Describe what the member gets |

## Miscellaneous

| Term | Guidelines |
| --- | --- |
| App / website | **App** = Included Health mobile app (iOS/Android). **Website** = www.includedhealth.com. Include the company name on first reference. If the device is unclear, say “the Included Health app or website.” |
| Button | Don’t refer to the element (“Select the Get started button”). Bold the label (“Select **Get started**”). If you can’t bold, use quotation marks. Tertiary buttons can look like links. |
| Login / log in | `login` / `logout` = noun or adjective (the login process). `log in` / `log out` = verbs. Members log in to / log out of the IH app. Use `log in` (two words, no hyphen), not `sign in` (too close to `sign up`). Use `log out`, not `log off`. |
| Signup / sign up | `signup` = noun/adjective for adding contact info to a bulletin (newsletter). `sign up` = verb for that act. Do not use `sign up` for creating an account — use **create account**. |
| Interface element names | Avoid naming UI parts when describing them: page, section, tab, button, icon, link, menu, card, sidebar. Refer to interface elements by their label, in bold. Do: "Select **Get started**." Don't: "Select the Get started button." |
