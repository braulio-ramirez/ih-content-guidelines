# Text fields

Members input or edit text. Other names: input, input field. Use a text area when more than one line is needed.

Form types, required fields, and validation timing live in [forms.md](forms.md).

## Labels

- Sentence case, not Title Case or ALL CAPS.
- Keep labels short.
- Required fields: asterisk after the label, with one space before it. Example: `First name *`
- Include a visible character limit only when users are likely to hit it. Don’t clutter every field with a counter.

## Placeholder text

- Format example only (e.g. `john@sample.com` for email).
- Do not put instructions in the placeholder. Instructions go in help text, which stays visible while editing.

## Help text

- Instructions the member may need while entering a value.
- Short, concise, meaningful.
- Sentence case **with** end punctuation.

## Error messages

- Shown when the input is incorrect or a required field is left blank. Validate live as the member fills in the field, and again on submit. See [forms.md](forms.md).
- Error text **replaces** help text until the error is cleared; then restore the original help text.
- Clear language. No ambiguity. No technical jargon (`404 error`, `Authentication failed`).
- Focus on what the member **can do** to fix it, not what they can’t do.
- Never blame the member. Tone rules for all error copy are in [ux-copy.md](../ux-copy.md) (Error messages).
- Sentence case **with** end punctuation.

## Copy that follows from usage

- If the member should be able to read the value, do not use disabled — use read-only.
- Never prevent typing past a character limit; prefer an error on submit unless an explicit counter is shown (typically text areas).
