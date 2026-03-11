# Guide 04: Track Your Posts

**What this covers:** How post tracking and the idea bank work, and what they reveal over time
**What Claude Code does:** Logs posts after each session, updates metrics when you share them, and surfaces ideas when you start a new post

---

## Why tracking matters

Most people post, watch the metrics for a day, and move on. Without a log, every post is a fresh start — you're guessing what works rather than building on what you know.

After 10-15 logged posts, patterns become visible:
- Which frameworks generate comments vs. likes
- Which topics attract the audience you actually want
- Which hook types perform for your specific audience
- Whether long or short posts work better for you

The data won't tell you everything, but it'll tell you enough to stop repeating mistakes and double down on what works.

---

## How post-log.md works

`post-log.md` is a simple table. Each row is one post.

After each `/lidev` session, Claude Code offers to add an entry with the date, topic, hook type, and framework used. When you publish the post, paste the LinkedIn URL back and it updates the entry.

A couple of days later, when you have metrics, tell Claude Code something like "my last post got 2,400 impressions and 18 comments" and it'll update the log. No form to fill out — just tell it the numbers.

**What gets tracked:**

| Field | What it captures |
|-------|----------------|
| Date | Published date |
| Topic | One-line description |
| Hook type | Story / Contrarian / Framework / Lesson / Other |
| URL | LinkedIn post URL |
| Impressions | From LinkedIn analytics (48-72 hrs) |
| Comments | Count, and note if high-quality |
| Notes | Anything worth remembering — unusual reach, unexpected audience, DMs generated |

---

## How idea-bank.md works

Ideas don't arrive on schedule. `idea-bank.md` is where they go when they do.

Anytime you have a post idea — in a conversation, reading something, after a meeting — just tell Claude Code: "Add this to my idea bank: [your idea]." It saves it.

When you start a new post session, Claude Code checks the idea bank and surfaces relevant topics before you decide what to write about.

**What makes a good idea entry:**

A rough note is fine — a sentence or two is enough to jog your memory later:

```
Had a call today where the client thought they had a process problem.
Turned out it was a people problem wearing a process costume.
Interesting reframe — worth a post.
```

---

## What the data tells you over time

After 15-20 posts, ask Claude Code to review your post log. It can identify:

- **Framework posts vs. story posts:** Which generates more comments? Comments indicate resonance — people respond when something lands.
- **Topic clusters:** Are certain topics generating 2x the impressions? You may have an audience primed for that area.
- **Hook types:** Is one hook type consistently outperforming others for your audience? That's your default starting point.
- **Post length:** Do longer posts trail off or hold attention?

Don't optimize too early. Wait until you have at least 10 comparable posts before drawing conclusions. One outlier will skew everything if you react to it.

---

Tracking in place. Next: `guide/05-voice-samples.md`
