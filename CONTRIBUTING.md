# Contributing

Thanks for adding to the pack. Contributions of any size are welcome; five templates in one category is the ideal first pull request.

## What makes a good template

1. **It is speakable in 30–60 seconds.** Read it out loud with a timer before submitting. If it runs long, cut fields — do not shorten the context sentence.
2. **It front-loads context.** The first sentence names who, what and when. This is non-negotiable: it is what makes the note survive without processing.
3. **It has square-bracket slots, not example text.** `[client code]`, not `"client 4471"`. Slots make it copy-paste ready.
4. **It ships with its prompt.** Every template needs the exact prompt that converts its transcript into the target output. The prompt must forbid invention — say what to do when a field is missing.
5. **It makes no legal, medical or compliance claim.** Templates for regulated professions describe a personal recap workflow only. Never state or imply that a workflow satisfies any regulation or professional obligation.

## Format

Match the existing structure exactly:

```markdown
### N.M — Short descriptive name

**Say this:**
> "Opening context sentence. [Field]: [slot]. [Field]: [slot]. ..."

**Then prompt with:**
```
The prompt. State the output structure. Forbid inventing missing values.
```
```

## Adding a new category

Open an issue first describing the profession or workflow and why the existing ten do not cover it. Categories need at least five templates to stand alone.

## Translations

Very welcome. Put them in `translations/<iso-code>/TEMPLATES.md` and keep the numbering identical to the English file so the two can be diffed. Translate the spoken parts; the prompts can stay in English or be translated, whichever works better for the target language.

## Licence

By contributing you agree your contribution is released under the MIT licence in `LICENSE`.
