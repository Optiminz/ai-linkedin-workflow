# Guide 03: Build Your Hook Bank

**What this covers:** How the hook bank works and why your hooks keep getting better
**What Claude Code does:** Suggests hooks from the bank during post sessions, and saves unused options back to the bank automatically

---

## What a hook is and why it matters

The first line of a LinkedIn post determines whether anyone reads the rest. LinkedIn truncates posts after two or three lines — the hook is everything above the fold.

A good hook does one of three things:

- **Creates tension:** Something is unresolved, counterintuitive, or surprising. "I spent three months building the wrong thing."
- **Implies a story:** There's something to find out. "The call lasted four minutes. By the end, we'd cut the project scope in half."
- **Challenges an assumption:** The reader's existing belief is put in question. "Most productivity advice is written for people who don't have much to do."

A weak hook describes what the post is about. A strong hook makes someone want to know what happens next.

---

## How the hook bank works

`hook-bank.md` stores hooks organized by type: story openings, contrarian takes, framework teasers, lessons-learned openers, and others.

When you run `/lidev`, Claude Code:

1. Reads your hook bank
2. Identifies hook types that fit your topic
3. Generates three options — each adapted to your content
4. Asks which direction you want to go

You pick one (or describe what you want from a combination), and the post develops from there.

After the session, any of the three options you didn't pick get offered back to the bank if they're strong enough to reuse in a different context. Claude Code handles this — it asks if you want to save them and updates the file.

---

## How it gets seeded

The bank comes pre-loaded with example hook structures to get you started. As you write more posts, it fills up with hooks tailored to your voice and topics.

You can also accelerate this by telling Claude Code:

- "Here are 5 LinkedIn posts I thought had great opening lines" — it'll extract the patterns and add them to your bank
- "I've posted before, here are my top 5 by engagement" — it'll pull the hook patterns from those
- "Add a hook structure for [specific pattern you like]"

You describe what you want. Claude Code creates the entries.

---

## Why it gets better over time

Every post session generates three hook options. You use one. The other two — if they're good — go into the bank. After 10-15 posts, you have a bank of 20-30 proven structures tuned to your voice, your topics, and your audience.

The system also learns which hook types perform best once you start tracking posts in `post-log.md`. It'll start favoring structures that generate engagement for your specific audience.

---

## Maintaining the bank

Every few months, it's worth reviewing the bank. You can ask Claude Code to:

- Remove hooks you've used once that didn't perform
- Keep any structure you've returned to more than twice
- Add variations when a hook works but felt slightly off

The bank isn't a library — it's a working tool. Keep it tight.

---

Got hooks. Next: `guide/04-track-your-posts.md`
