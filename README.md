# Alfred-workflow-copy-selected-text-to-TextEdit
This simple demonstration workflow is designed to enable spellcheck of selected text which (for one reason or another) is not subject to spell checking in its original app.

A Universal Action takes the selected text, TextEdit is opened (so it's the frontmost app), the selected text is passed to the clipboard. The `Copy to clipboard` action has both of these options checked:

- `Automatically paste to frontmost app` (because we've ensured TextEdit is the frontmost app)

- `Mark item as transient in clipboard` (because you presumably don't want chunks of text hanging around on the clipboard).

TextEdit should highlight any words it consider misspelled—then, of course, it's up to you close TextEdit and choose not to save anything.
