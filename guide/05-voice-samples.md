# Guide 05: Voice Samples

**What this covers:** Why voice samples matter and how to provide better ones
**What Claude Code does:** Analyzes your samples, extracts patterns, and saves structured voice profiles automatically

---

## Why the Constitution isn't enough on its own

The Constitution defines boundaries. No "leverage." Measured intensity. Conversational professional.

But rules describe the absence of bad, not the presence of good. Sentence rhythm, the way you open a thought, how much you compress before you expand — that comes from examples. A voice sample gives the AI something to pattern-match against, not just avoid.

---

## How it works

During your first session, Claude Code asks you to paste writing samples and creates a voice profile from them. That profile lives in `voice-samples/` and gets loaded every time you write a post.

To add more samples later, just paste them into a Claude Code session and say "add this as a voice sample." It handles the analysis and file creation.

---

## How to pick good samples

Go through things you've written — LinkedIn posts, emails, documents, Slack messages. Look for ones where you re-read them and think: yes, that's actually how I think.

Good signs:
- You used a phrase you wouldn't see anywhere else
- It makes a point that only you would make in that way
- The rhythm feels natural when you read it aloud

Bad signs:
- You already suspect AI helped too much
- It reads like it could have been written by anyone in your field
- It's technically correct but a bit flat

---

## How many samples

3-5 is a working minimum. More is better — up to around 10-12 before diminishing returns set in.

Varied topics are fine. Voice consistency matters more than topical consistency. A sample about your morning routine and a sample about pricing strategy can both be useful if they both sound like you.

---

## What the system looks for in your samples

When you run `/lidev`, Claude Code reads your voice samples and looks at:

- How you open — do you lead with an observation, a question, a statement of fact?
- Sentence length variation — long, then short. Or always compressed. Or flowing.
- Word-level choices — the specific language you reach for
- How you close — do you ask something, state something, leave it hanging?

The samples don't get copied. They get read for pattern.

---

## Improving your profile over time

After a few posts, if something still feels off, you can:

- Paste more samples: "Here's an email I wrote that really sounds like me"
- Flag specific patterns: "I notice I always use short sentences after making a big claim — protect that"
- Remove samples that aren't representative anymore

Tell Claude Code what you want changed. It updates the voice profile files.

---

Voice dialed in. Next: `guide/06-content-strategy.md`
