# Negotiation Arena configuration

Editable case, rule, prompt and participant-guide files for Negotiation Arena.

## Neggy and persistent counterpart bargaining

`ai-prompts.json` includes the stay-at-the-table instructions under `modules.counterpart`. Import a reviewed prompt pack through the app admin controls; existing sessions retain their frozen pack. The server also enforces warning-before-withdrawal.

`neggy-guide.json` contains tutorial copy. It is compiled interface text, so edits need an app rebuild and deployment. It is not a live AI-prompt importer. The private admin mechanics guide documents closure, warning, review-unlock and attribution rules.
