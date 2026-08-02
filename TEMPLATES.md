# Voice Note Templates — all 50

> Web version with anchors and formatting: https://pittner.github.io/voice-note-templates/

Each template has two parts: **Say this** (what you speak, 30–60 seconds) and **Then prompt with** (the prompt you run on the transcript). Square brackets are slots you fill as you talk.

---

## 1. Meetings & standups

*The goal of a post-meeting memo is not a record of the meeting. It is the list of things that changed. Say the decisions and the owners; skip the discussion.*

### 1.1 — Post-meeting decision log

**Say this:**

> “Meeting recap. [Project], [date], attendees [names]. Three decisions were made. One: [decision], owner [name], by [date]. Two: [decision], owner, date. Three: [decision], owner, date. One thing is still open: [question], and [name] owes us an answer by [date].”

**Then prompt with:**

```
Turn this transcript into two lists: DECISIONS (one line each, no discussion) and OPEN QUESTIONS (question, who owes the answer, by when). Do not invent owners or dates. If one is missing, write UNASSIGNED.
```

### 1.2 — Action items only

**Say this:**

> “Action items from [meeting]. I owe [name] the [deliverable] by [day]. [Name] owes me [deliverable] by [day]. Nobody owns [item] yet — flag it.”

**Then prompt with:**

```
Extract every action item as: owner, deliverable, due date, blocked-by. Output as a checklist. Mark items with no owner as UNASSIGNED at the top of the list.
```

### 1.3 — Standup, spoken on the walk in

**Say this:**

> “Standup for [date]. Yesterday I finished [x] and got stuck on [y]. Today I am doing [z]. My blocker is [blocker] and the person who can unblock it is [name].”

**Then prompt with:**

```
Format as three bullets: Yesterday, Today, Blockers. Under Blockers, name the person who can unblock each item. Keep it under 60 words.
```

### 1.4 — The meeting that should have been an email

**Say this:**

> “Summary for people who were not there. The one thing you need to know is [x]. It affects you if [condition]. If it affects you, do [action] by [date]. Otherwise ignore this.”

**Then prompt with:**

```
Rewrite as a short internal update email. Lead with the one thing that matters. Second paragraph: who is affected and what they must do. No greeting fluff, no recap of the agenda.
```

### 1.5 — Interview or 1:1 debrief

**Say this:**

> “Debrief, [name], [role], [date]. Strongest signal: [evidence]. Weakest signal: [evidence]. One thing I still do not know: [gap]. My recommendation right now is [advance / hold / decline] and my confidence is [low / medium / high].”

**Then prompt with:**

```
Structure as: Signal for, Signal against, Open gap, Recommendation with confidence level. Quote the evidence given, do not add reasoning of your own.
```

Longer write-up of this workflow: [turning meeting voice notes into action items](https://voxflow.bemooore.com/blog/meeting-notes-voice-to-action-items/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 2. Sales calls, showings & field visits

*The recap you record in the car park is worth more than the one you type at 7pm, because at 7pm you have lost the objection wording. Record before you start the engine.*

### 2.1 — Car-park recap after a client visit

**Say this:**

> “Visit recap. [Company], [contact name and role], [date]. What they are trying to fix: [problem in their words]. Budget signal: [what they said about money]. Timeline signal: [when]. Objection raised: [objection, quoted]. Next step I committed to: [action] by [date].”

**Then prompt with:**

```
Convert to a CRM entry with fields: Account, Contact, Pain (their words), Budget signal, Timeline, Objection (verbatim), Next step, Due date. Leave a field blank rather than guessing.
```

### 2.2 — Property showing recap

**Say this:**

> “Showing recap. [Address], [date], buyers [names]. They reacted well to [feature] and badly to [feature]. Their real constraint sounded like [constraint]. Competing property they mentioned: [property]. My next action: [action] by [date].”

**Then prompt with:**

```
Summarise as: Positive reactions, Negative reactions, Stated constraint, Competing options mentioned, Next action with date. Then suggest two follow-up properties criteria based only on what was said.
```

### 2.3 — Objection capture

**Say this:**

> “Objection log. [Company]. The objection, in their exact words, was: [quote]. The context was [when in the call it came up]. What I answered: [answer]. Whether it landed: [yes / no / unclear].”

**Then prompt with:**

```
Add this to an objection library entry: Objection (verbatim), Context, Response given, Outcome. Then list two alternative responses, each under 30 words.
```

### 2.4 — Pipeline hygiene sweep

**Say this:**

> “Pipeline check, [date]. [Account] — last contact [date], real next step [step], my honest confidence [percent]. [Account] — same three fields. [Account] — same three fields. The one I am kidding myself about is [account].”

**Then prompt with:**

```
Output a table: Account, Days since last contact, Concrete next step, Stated confidence. Add a final row listing the account the speaker flagged as self-deception, with the reason if given.
```

### 2.5 — Handover to a colleague

**Say this:**

> “Handover, [account], to [colleague]. Relationship status: [status]. Who actually decides: [name and role]. What you must not say: [landmine]. What is promised and when: [promise]. First thing you should do: [action].”

**Then prompt with:**

```
Write a handover note for the incoming rep: Status, Decision maker, Sensitivities to avoid, Outstanding promises with dates, Recommended first action. Flag anything that is a commitment the company must honour.
```

Longer write-up: [voice notes for field sales and realtors](https://voxflow.bemooore.com/blog/voice-notes-for-field-sales-realtors/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 3. Client sessions & private practice

*These templates are recorded *after* the client has left — they are your recap, not a recording of the session, so no consent question arises. Check your own professional record-keeping obligations before adopting any workflow.*

### 3.1 — Session recap, structured

**Say this:**

> “Session recap, client [initials or code], [date], session number [n]. Presenting focus today: [topic]. What changed since last time: [change]. What I observed: [observation]. What we agreed for next time: [agreement]. My own note to self: [note].”

**Then prompt with:**

```
Structure as: Focus, Change since last session, Observations, Agreed next steps, Clinician note. Keep the client identifier exactly as spoken. Do not add interpretation that was not stated.
```

### 3.2 — Between-session observation

**Say this:**

> “Observation, client [code], [date]. I noticed [pattern] across the last [n] sessions. The first time I saw it was [when]. What I want to test next session is [approach].”

**Then prompt with:**

```
Write as a single dated progress note: Pattern observed, Evidence across sessions, Planned approach. No diagnosis language unless it was spoken.
```

### 3.3 — Referral or coordination note

**Say this:**

> “Coordination note. Client [code]. I want to refer to [discipline] because [reason]. Relevant history in one sentence: [history]. What I need back from them: [question].”

**Then prompt with:**

```
Draft a short professional referral summary: Reason for referral, Relevant background (one sentence), Specific question being asked. Neutral clinical tone, no speculation.
```

### 3.4 — End-of-day caseload sweep

**Say this:**

> “End of day, [date]. [n] sessions. The one I am still thinking about is [code], because [reason]. Admin I owe: [items]. Supervision topic to raise: [topic].”

**Then prompt with:**

```
Output three lists: Cases needing further thought (with the stated reason), Admin owed, Supervision agenda items. Nothing else.
```

### 3.5 — Cancellation and no-show log

**Say this:**

> “Attendance note. Client [code], [date], [cancelled / no-show], notice given [amount]. Reason stated: [reason]. Pattern so far: [nth occurrence]. Action: [rebook / discuss / policy].”

**Then prompt with:**

```
Log as: Client code, Date, Type, Notice, Stated reason, Occurrence count, Action taken. Flag if the occurrence count is three or higher.
```

Longer write-up: [voice notes for therapists and clinicians](https://voxflow.bemooore.com/blog/voice-notes-for-therapists-clinicians/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 4. Legal matter recaps

*Again: these are your own post-call recaps, not recordings of the other party. Retention, privilege and record-keeping rules are yours to check — this pack takes no position on them.*

### 4.1 — Post-call matter recap

**Say this:**

> “Matter recap. [Matter reference], [date], call with [party]. What they want: [position]. What they conceded: [concession]. What is now disputed: [issue]. Deadline created by this call: [date]. My next step: [action].”

**Then prompt with:**

```
Structure as: Matter reference, Counterparty position, Concessions, Live disputes, Deadlines created, Next steps. Preserve dates exactly. Do not characterise anything as agreed unless the word agreed was used.
```

### 4.2 — Time entry, spoken

**Say this:**

> “Time entry. Matter [reference], [date]. Task: [description]. Duration: [minutes]. Billable: [yes / no]. Narrative: [one sentence a client would accept].”

**Then prompt with:**

```
Produce a billing narrative line: matter reference, date, duration, and a one-sentence description written in client-facing language. No internal shorthand.
```

### 4.3 — Document review note

**Say this:**

> “Review note. Document [name], matter [reference]. The clause that matters is [clause] because [reason]. Risk level: [high / medium / low]. Change I would ask for: [redline].”

**Then prompt with:**

```
Output: Document, Clause, Why it matters, Risk level, Proposed change. If a risk level was stated, keep it; never assign one that was not spoken.
```

### 4.4 — Deadline capture

**Say this:**

> “Deadline. Matter [reference]. The date is [date]. It is triggered by [event]. What must be filed or served: [item]. Who is doing it: [name]. Buffer I want: [days].”

**Then prompt with:**

```
Create a calendar entry: title, hard date, trigger event, deliverable, owner, and a reminder date calculated by subtracting the stated buffer. Show the arithmetic.
```

### 4.5 — Client update draft

**Say this:**

> “Client update, matter [reference]. Since we last spoke: [event]. What it means for them: [implication, plain language]. What I need from them: [request] by [date]. What happens next: [next step].”

**Then prompt with:**

```
Draft a client-facing update email in plain language, no Latin, no jargon. Four short paragraphs matching the four fields. End with the requested item and its date in bold.
```

Longer write-up: [voice notes for attorneys and lawyers](https://voxflow.bemooore.com/blog/voice-notes-for-attorneys-lawyers/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 5. Lectures, seminars & study

*Recording the whole lecture creates 50 minutes you will never replay. A 60-second recap recorded while walking out is the artefact you will actually revise from.*

### 5.1 — Walking-out lecture recap

**Say this:**

> “Lecture recap. [Course], [topic], [date]. The single claim was [claim]. The evidence given was [evidence]. The thing I did not understand is [gap]. What is examinable here is probably [prediction].”

**Then prompt with:**

```
Format as: Central claim, Supporting evidence, Comprehension gap, Likely exam angle. Then generate three recall questions with answers, based only on the transcript.
```

### 5.2 — Reading note

**Say this:**

> “Reading note. [Source], [author], pages [range]. The argument is [argument]. What it disagrees with is [counter-position]. The quote I want is on page [n]: [quote]. How it connects to [other source]: [connection].”

**Then prompt with:**

```
Output a literature note: Source, Argument, Position it opposes, Key quote with page number, Connection to other reading. Preserve the page numbers exactly.
```

### 5.3 — Flashcard dump

**Say this:**

> “Flashcards for [topic]. Term [term], definition [definition]. Term, definition. Term, definition. The one I keep getting wrong is [term].”

**Then prompt with:**

```
Output as a two-column CSV: front, back. Add a third column priority, set to high for the term the speaker said they keep getting wrong, normal for the rest.
```

### 5.4 — Pre-exam confidence sweep

**Say this:**

> “Exam sweep, [subject], [days] days out. Confident on [topics]. Shaky on [topics]. No idea on [topics]. Time available: [hours].”

**Then prompt with:**

```
Build a revision plan allocating the stated hours across the three confidence bands, weighted towards no-idea then shaky. Show the allocation as a table with hours per topic.
```

### 5.5 — Seminar contribution prep

**Say this:**

> “Seminar prep, [topic]. The point I want to make is [point]. The evidence I will cite is [evidence]. The obvious counter is [counter] and my response is [response].”

**Then prompt with:**

```
Write this as speaking notes: one-sentence point, one-sentence evidence, anticipated counter, prepared response. Under 100 words total so it can be read at a glance.
```

Longer write-up: [voice to text for lectures and study notes](https://voxflow.bemooore.com/blog/voice-to-text-lecture-study-notes/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 6. Writing & first drafts

*Speaking is roughly three times faster than typing, and a spoken draft carries your actual cadence. The trick is to dictate the *argument*, not the prose.*

### 6.1 — Spoken outline before writing

**Say this:**

> “Outline for [piece]. The reader is [audience]. After reading it they should [change]. My argument in one sentence: [thesis]. The three moves are: [move one], [move two], [move three]. The thing I must not forget: [detail].”

**Then prompt with:**

```
Turn this into a working outline: audience, desired change, thesis, three sections with a one-line purpose each, and a note list. Do not write any prose yet.
```

### 6.2 — Talk-it-out first draft

**Say this:**

> “First draft, [piece]. Opening: [say the opening as you would say it to a friend]. Middle: [the argument, out loud, unpolished]. Ending: [the point you want to land].”

**Then prompt with:**

```
Clean this transcript into a readable first draft. Keep the speaker's word choice and rhythm. Remove filler words, false starts and repetitions only. Do not add ideas, examples or transitions that were not spoken.
```

### 6.3 — Email you are dreading

**Say this:**

> “Email to [recipient]. What I actually want is [want]. What I am worried about is [worry]. What I am willing to concede is [concession]. Tone should be [tone].”

**Then prompt with:**

```
Draft the email in the stated tone. Lead with the ask, not the apology. Include the concession only if it strengthens the ask. Under 150 words.
```

### 6.4 — Idea capture with enough context to survive

**Say this:**

> “Idea, [date]. The idea is [idea]. It came from [trigger]. Who it would be for: [audience]. The first thing I would have to test is [test]. The reason it might be nothing: [risk].”

**Then prompt with:**

```
Store as: Idea, Trigger, Audience, First test, Stated risk. Then write one sentence I could read in six months that would let me reconstruct why this seemed interesting.
```

### 6.5 — Revision pass, spoken

**Say this:**

> “Revision notes for [piece]. What works: [section]. What does not: [section] because [reason]. What is missing: [gap]. What I should cut even though I like it: [darling].”

**Then prompt with:**

```
Produce a revision checklist ordered by impact: cuts first, then fixes, then additions. Include the stated reason next to each item.
```

Longer write-up: [from voice memo to first draft](https://voxflow.bemooore.com/blog/voice-memo-to-first-draft/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 7. Journaling & brain dumps

*Written journaling fails on the days it would help most, because on those days you have no patience for a blank page. Speaking has almost no activation cost.*

### 7.1 — Ninety-second brain dump

**Say this:**

> “Brain dump, [date]. Everything currently in my head: [say it unfiltered until you run out]. The one that is actually urgent is [item]. The one that is loud but not important is [item].”

**Then prompt with:**

```
Split into three lists: Actionable (with a suggested next physical action each), Waiting on someone else, Noise. Put the item the speaker called urgent at the top of Actionable.
```

### 7.2 — Evening review

**Say this:**

> “Evening review, [date]. What actually happened: [events]. What I did well: [thing]. What I would redo: [thing]. Energy level and why: [level, cause]. Tomorrow's single most important thing: [task].”

**Then prompt with:**

```
Write as a dated journal entry in first person, keeping the speaker's phrasing. End with a line: TOMORROW — followed by the single most important task.
```

### 7.3 — Decision journal

**Say this:**

> “Decision, [date]. I decided [decision]. The alternatives were [options]. I chose this because [reasoning]. What I expect to happen: [prediction]. When I will check: [date]. Confidence: [percent].”

**Then prompt with:**

```
Record as a decision-journal entry with fields: Decision, Alternatives, Reasoning, Prediction, Review date, Confidence. Do not evaluate the decision.
```

### 7.4 — Emotional first aid

**Say this:**

> “Right now I feel [feeling]. It started when [trigger]. The story I am telling myself is [story]. What is actually verifiable is [facts]. The smallest useful next action is [action].”

**Then prompt with:**

```
Reflect back four sections: Feeling, Trigger, Interpretation, Verifiable facts, Smallest next action. Do not offer advice, reassurance or diagnosis. Use the speaker's own words wherever possible.
```

### 7.5 — Weekly pattern check

**Say this:**

> “Week of [date]. The pattern I noticed in myself was [pattern]. It showed up on [days]. What preceded it each time: [antecedent]. One experiment for next week: [experiment].”

**Then prompt with:**

```
Summarise as: Pattern, Occurrences, Common antecedent, Experiment. Then propose one measurable success criterion for the experiment.
```

Longer write-up: [voice journaling and brain dump workflows](https://voxflow.bemooore.com/blog/voice-journaling-brain-dump-app/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 8. Travel & multilingual capture

*Two constraints stack when travelling: no reliable connection, and thoughts arriving in whichever language you are currently living in. Templates that name the language up front save the transcript.*

### 8.1 — Language-tagged capture

**Say this:**

> “Note in [language], [date], [place]. [Then say the note entirely in that language, without switching.]”

**Then prompt with:**

```
Transcribe in the original language. Then provide an English summary underneath, marked SUMMARY. Never mix the two in one paragraph.
```

### 8.2 — Field observation abroad

**Say this:**

> “Field note. [Place], [date], [time]. What I am looking at: [description]. What surprised me: [surprise]. What I want to look up later: [question]. Photo reference: [filename or count].”

**Then prompt with:**

```
Format as a dated field note: Location, Observation, Surprise, Follow-up question, Media reference. Keep place names spelled as spoken.
```

### 8.3 — Expense capture on the move

**Say this:**

> “Expense. [Amount] [currency], [date], [merchant], [category]. Business purpose: [purpose]. Receipt: [have it / lost it]. Project code: [code].”

**Then prompt with:**

```
Output one expense row: Date, Amount, Currency, Merchant, Category, Business purpose, Receipt status, Project code. Flag rows where receipt status is lost.
```

### 8.4 — Interpreter-free meeting recap

**Say this:**

> “Meeting recap in [language]. [Name], [company], [date]. Agreed: [points]. Unclear because of language: [points]. Follow up in writing: [items].”

**Then prompt with:**

```
Produce two sections: CONFIRMED (things stated as agreed) and TO CONFIRM IN WRITING (anything the speaker flagged as unclear). Translate to English but keep any quoted phrases in the original.
```

### 8.5 — Airplane-mode idea log

**Say this:**

> “Offline note, [date], flight [number or route]. Idea: [idea]. Why now: [trigger]. What I need to check when I land: [checks].”

**Then prompt with:**

```
Store as: Idea, Trigger, To verify on landing. Output the verification items as a checklist so they can be worked through in order.
```

Longer write-up: [voice to text in any language, offline](https://voxflow.bemooore.com/blog/voice-to-text-any-language-offline/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 9. Wrist & hands-free capture

*The value of wrist capture is not convenience, it is the elimination of the phone. If getting the idea down requires unlocking a device and choosing an app, the idea is gone. Wrist templates must therefore be short enough to say in one breath.*

### 9.1 — One-breath capture

**Say this:**

> “[Noun phrase for the idea]. Because [one reason]. Next: [one action].”

**Then prompt with:**

```
Expand into a single note: Idea, Rationale, Next action. Do not pad. If the transcript is ambiguous, list the ambiguity instead of resolving it.
```

### 9.2 — Mid-walk task capture

**Say this:**

> “Task. [Task]. For [project]. By [day]. Blocked by [nothing / thing].”

**Then prompt with:**

```
Output one task line: description, project, due date, blocker. If blocker is nothing, omit the field entirely.
```

### 9.3 — Driving recap (stationary, engine off)

**Say this:**

> “Recap. [Who I just met]. [The one thing that changed]. [The one thing I owe them]. [When].”

**Then prompt with:**

```
Four fields only: Person, What changed, Commitment, Deadline. This is a car-park note, keep the output equally short.
```

### 9.4 — Workout or run note

**Say this:**

> “Session [date]. Did [work]. Felt [rating out of ten]. Niggle: [body part or none]. Next session should be [adjustment].”

**Then prompt with:**

```
Log as: Date, Work completed, Perceived effort, Niggle, Adjustment for next session. Track niggles as a separate running list across entries.
```

### 9.5 — Shopping and errands

**Say this:**

> “Errands. Buy [items]. From [shop]. Before [day], because [reason].”

**Then prompt with:**

```
Output a grouped shopping list by shop, with a deadline line at the top. Merge duplicate items.
```

Longer write-up: [the Apple Watch voice memo workflow](https://voxflow.bemooore.com/blog/apple-watch-voice-memo-ai-workflow/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## 10. Leaving a subscription transcription tool

*Most people who cancel a transcription subscription do not miss the transcription — they miss the templates the tool had baked in. These five replace the ones that actually got used.*

### 10.1 — Migration inventory

**Say this:**

> “Migration note. I am leaving [tool]. What I used it for, honestly: [uses]. What I never used: [features]. What I must not lose: [data]. Export deadline: [date].”

**Then prompt with:**

```
Produce: Actually-used features, Never-used features, Data that must be exported, Export deadline. Then list what a replacement must do, based only on the actually-used list.
```

### 10.2 — What it was really costing

**Say this:**

> “Cost check. [Tool], [amount] per [month or year], [months] used. Times I opened it last month: [number]. Cost per actual use: [say the division out loud or leave it].”

**Then prompt with:**

```
Compute annualised cost, cost per opening, and cost per opening projected over twelve months. Show the arithmetic. Do not recommend anything.
```

### 10.3 — Privacy requirements, written down once

**Say this:**

> “Requirements. Audio must [leave / not leave] the device. Transcripts stored [where]. Retention [duration]. Sharing with third parties: [acceptable / not]. Offline capability: [required / nice to have].”

**Then prompt with:**

```
Turn into a requirements checklist with must-have and nice-to-have columns. Keep the wording literal — these are procurement criteria, not a legal or compliance assessment.
```

### 10.4 — Trial evaluation, spoken

**Say this:**

> “Trial day [n] of [tool]. What worked: [thing]. What annoyed me: [thing]. Did it survive my worst case, which is [worst case]: [yes / no]. Would I pay: [yes / no] and why.”

**Then prompt with:**

```
Log as a dated trial entry: Worked, Annoyed, Worst-case result, Willingness to pay with reason. Across multiple entries, surface any annoyance mentioned more than once.
```

### 10.5 — Team rollout note

**Say this:**

> “Rollout. Replacing [tool] with [tool] for [team]. Who is affected: [names or roles]. What breaks on day one: [things]. Training needed: [amount]. Rollback plan: [plan].”

**Then prompt with:**

```
Write a short rollout plan: Scope, Affected people, Day-one breakage, Training, Rollback trigger and plan. One page maximum.
```

Longer write-ups: [subscription-free alternatives to cloud transcription](https://voxflow.bemooore.com/blog/otter-alternative-no-subscription/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates) and [free offline voice to text on iPhone and Mac](https://voxflow.bemooore.com/blog/free-offline-voice-to-text-iphone-mac/?utm_source=github&utm_medium=referral&utm_campaign=voice_note_templates).

---

## Licence

MIT — see [`LICENSE`](LICENSE). Contributions welcome, see [`CONTRIBUTING.md`](CONTRIBUTING.md).
