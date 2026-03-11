# Guide 05: Voice Samples

**Why you're here:** Your posts sound polished but not quite like you. Rules tell the AI what to avoid — samples show it what to aim for.

---

## Why the Constitution isn't enough on its own

The Constitution defines boundaries. No "leverage." Measured intensity. Conversational professional.

But rules describe the absence of bad, not the presence of good. Sentence rhythm, the way you open a thought, how much you compress before you expand — that comes from examples. A voice sample gives the AI something to pattern-match against, not just avoid.

---

## How to pick good samples

Go through posts you've written — on LinkedIn, in emails, in documents. Look for ones where you re-read them and think: yes, that's actually how I think.

Good signs:
- You used a phrase you wouldn't see anywhere else
- It makes a point that only you would make in that way
- The rhythm feels natural when you read it aloud

Bad signs:
- You already suspect AI helped too much
- It reads like it could have been written by anyone in your field
- It's technically correct but a bit flat

---

## How many samples to include

3–5 is a working minimum. More is better — up to around 10–12 before diminishing returns set in.

Varied topics are fine. Voice consistency matters more than topical consistency. A sample about your morning routine and a sample about pricing strategy can both be useful if they both sound like you.

---

## How the system uses them

When you run `/lidev`, the system reads your voice samples before generating anything. It looks at:

- How you open — do you lead with an observation, a question, a statement of fact?
- Sentence length variation — long, then short. Or always compressed. Or flowing.
- Word-level choices — the specific language you reach for
- How you close — do you ask something, state something, leave it hanging?

The samples don't get copied. They get read for pattern.

---

## Where to save them

Create files in the `voice-samples/` directory:

```
voice-samples/
  yourname-topic.md
  yourname-another-topic.md
```

Keep file names simple and descriptive. The content of each file should just be the post text itself — no markup, no headers, no metadata.

---

## What each sample file looks like

Just the text. Nothing else required.

```
Three years ago I thought onboarding was a checklist problem.

It's not. It's a trust problem. The checklist is just where trust either forms or doesn't.

We started treating the first two weeks less like task completion and more like relationship building. Fewer forms. More conversations about what success actually looks like for this person.

Retention went up. But more usefully, we stopped losing people we didn't know were about to leave.

---

[Note: this one works because of the pivot in line two — "it's not X, it's Y" is a structure worth repeating]
```

The note at the bottom is optional. Include it if there's something specific about the sample worth flagging to the AI — a structure you like, a phrase pattern you want more of.

---

Voice dialed in. Next: `guide/06-content-strategy.md`
