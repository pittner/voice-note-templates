# Voice Note Templates

**50 free, MIT-licensed templates for spoken notes.** Each one tells you exactly what to say into your phone or watch in 30–60 seconds, and gives you the AI prompt that turns the transcript into something usable: meeting action items, a CRM entry, a session recap, study notes, or a first draft.

📖 **Read the full pack: https://pittner.github.io/voice-note-templates/**

---

## The problem these solve

Most people abandon voice notes for the same reason: the transcript comes back as one unpunctuated paragraph that takes longer to read than the thing would have taken to type.

That is not a transcription-quality problem. It is a **structure** problem — nobody said the fields out loud, so nothing downstream can find them. No summariser, no search, and not you in three weeks.

A template fixes it in the cheapest possible place: the 45 seconds you were already spending.

## The method

1. **State the context first** — who, what, when, in the opening sentence. This is the step everyone skips and the one that matters most. A note that starts with context is routable even if you never process it further.
2. **Speak the template body** — 30 to 60 seconds. Longer memos ramble and summarise badly; shorter ones drop the context.
3. **Run the matching prompt on the transcript** — every template ships with the exact prompt for its output format.

## The ten categories

| # | Category | Typical output |
|---|----------|----------------|
| 1 | Meetings & standups | Decision log, action items, standup update |
| 2 | Sales calls, showings & field visits | CRM entry, objection library, handover note |
| 3 | Client sessions & private practice | Structured session recap, referral note |
| 4 | Legal matter recaps | Matter recap, time entry, deadline capture |
| 5 | Lectures, seminars & study | Recall questions, literature notes, flashcards |
| 6 | Writing & first drafts | Outline, cleaned first draft, revision checklist |
| 7 | Journaling & brain dumps | Sorted brain dump, decision journal, evening review |
| 8 | Travel & multilingual capture | Language-tagged notes, expense rows, field notes |
| 9 | Wrist & hands-free capture | One-breath capture, task line, car-park recap |
| 10 | Leaving a subscription tool | Migration inventory, cost check, requirements list |

Full text of all 50: [`TEMPLATES.md`](TEMPLATES.md) or the [web version](https://pittner.github.io/voice-note-templates/).

## Example

**Say this (category 1, post-meeting decision log):**

> "Meeting recap. Project Atlas, 12 March, attendees Sam and Priya. Three decisions were made. One: we ship without the import feature, owner Sam, by 20 March. Two: pricing stays as is until Q3, owner Priya, no date. Three: we drop the Android build, owner me, by 15 March. One thing is still open: who owns migration support, and Priya owes us an answer by 14 March."

**Then prompt with:**

```
Turn this transcript into two lists: DECISIONS (one line each, no discussion)
and OPEN QUESTIONS (question, who owes the answer, by when). Do not invent
owners or dates. If one is missing, write UNASSIGNED.
```

## Which app?

Any of them. The templates are plain text on purpose — built-in dictation on iOS, macOS and Android all work, as does any transcription service.

The one property worth deciding deliberately is **where the audio goes**, because it is the only one you cannot change afterwards:

| | Cloud transcription | On-device transcription |
|---|---|---|
| Works in airplane mode | No | Yes |
| Audio uploaded to a third party | Yes, by design | No — processing is local |
| Minutes cap | Common on free tiers | Bounded by device, not plan |

> "On-device" is a technical statement about where processing runs. It is not a legal or compliance claim, and nothing in this pack should be read as one.

These templates were written alongside [VoxFlow](https://voxflow.bemooore.com/) — free, no account, on-device speech model, iPhone / Mac / Apple Watch, 99 languages, works offline. You do not need it to use anything here.

## Contributing

PRs welcome, especially for professions the ten categories miss — nurses, surveyors, inspectors, teachers, social workers, veterinarians. See [`CONTRIBUTING.md`](CONTRIBUTING.md). Five templates in the existing format is the right size for a first PR.

## Licence

MIT — see [`LICENSE`](LICENSE). Copy them, fork them, translate them, ship them inside your own product docs.
