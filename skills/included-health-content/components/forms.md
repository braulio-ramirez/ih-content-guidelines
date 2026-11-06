# Forms

Forms collect information from the member. Field-level rules (labels, placeholders, help text, error text) live in [text-fields.md](text-fields.md). Checkbox and radio rules live in their own files. Source: Product Content Style Guide (Google Doc), Forms section.

## Form types

| Type | Questions | Button | Required markers |
| --- | --- | --- | --- |
| Standard form | One or more questions | **Submit** | Shown |
| Express form | One question per screen | **Next** | Not shown |

Button labels follow [buttons.md](buttons.md).

## Required fields

- Mark a required field with an asterisk after the label, with one space before it: `First name *` (see [text-fields.md](text-fields.md)).
- Standard forms show the legend `* = required field` at the top of the form.
- Express forms do not show required markers.
- Make the required input format clear in the label or help text.

## Labels and placeholders

- Label fields clearly and concisely. Sentence case, not all caps: `Card number`, not `CARD NUMBER`.
- Placeholders show a format example only, such as `john@sample.com` (see [text-fields.md](text-fields.md)). Describe what to enter in the label or help text.

## Validation

- Validate live, as the member fills in the field.
- Validate again on submit.
- When input is incorrect, show a clear error message. Error copy follows [text-fields.md](text-fields.md) (error messages) and [ux-copy.md](../ux-copy.md) (error messages).
