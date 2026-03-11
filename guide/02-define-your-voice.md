# Guide 02: Define Your Voice

**What this covers:** How the Editorial Constitution works and why it matters
**What Claude Code does:** Analyzes your writing samples and configures the Constitution automatically during setup

---

## What the Editorial Constitution does

`EDITORIAL-CONSTITUTION.md` is the rulebook every prompt in this system reads before generating anything. It defines your voice in three ways:

1. **Voice dimensions** — measurable settings on tone and style scales
2. **AI Tells** — words and phrases that feel wrong in your writing
3. **Keep List** — patterns that are distinctly yours, worth protecting

Without this file configured, the AI defaults to generic LinkedIn voice. With it, the AI has specific constraints to work inside.

---

## How it gets set up

When you first run Claude Code in this repo, it asks you to paste writing samples. From those samples, it automatically:

- Sets your voice dimensions (intensity, humor, formality)
- Identifies AI Tells to avoid — phrases that would sound wrong in your voice
- Builds your Keep List — patterns that are distinctly yours

You don't open the file and fill in blanks. Claude Code reads your writing, proposes the settings, and saves them after you confirm.

---

## What the voice dimensions mean

### Intensity (1-10)
How strong is your language?

- **2-3:** Understated, measured. "This approach tends to work." "Worth considering."
- **4-5:** Confident without hype. "This works." "Strong choice for most situations."
- **6-7:** Emphatic. "This is the move." "Don't skip this."
- **8-10:** High-energy. "Absolute game changer." "This will transform how you work."

Most professional writers sit at 4-6.

### Funny / Serious (1-5)
- **1-2:** Dry, deadpan, or openly playful. Jokes land. Wit is part of the brand.
- **3:** Occasional light touch — a phrase here, an observation there.
- **4-5:** Mostly or entirely serious. Warmth is fine; humor is rare.

### Formal / Casual (1-5)
- **1-2:** Conversational. "Here's the thing." "Honestly." "You probably already know this."
- **3:** Professional but human. Full sentences, no slang, but not stiff.
- **4-5:** Formal. Would work in a report or whitepaper without edits.

---

## What AI Tells are

AI Tells are words and phrases that sound fine in theory but feel wrong when you read them in your own voice.

Common ones across most writers:
- delve, unlock, leverage, seamless, game-changing, bustling, elevate
- "Here's the kicker," "Here's what nobody tells you," "Let's dive in"
- "In today's fast-paced world," "As we navigate [topic]"
- Any sentence starting with "It's important to note that"

Claude Code identifies these from your writing samples (by noticing what's absent from your natural voice) and adds them to the Constitution. The list grows over time — if something slips through in a future session, just tell Claude Code and it'll add it.

---

## What the Keep List protects

AI tools smooth out distinctive patterns in an attempt to sound "good." The Keep List protects the patterns that make your writing yours.

Examples of what a Keep List entry might look like:
- "Uses approximate language — 'around 80%' not '79.4%'"
- "Names specific tools and products, doesn't say 'a popular platform'"
- "Frames mistakes as learning: 'learned the hard way' not 'discovered'"
- "Occasional wordplay pattern: [less X, more Y]"

Again — Claude Code builds this from your samples. You review and refine it over time.

---

## Fine-tuning later

After a few posts, you'll notice things the Constitution doesn't catch yet. Just tell Claude Code:

- "That phrase sounds too corporate, add it to the AI Tells list"
- "I like how I use short one-line paragraphs for emphasis — protect that"
- "My intensity should be more like a 5, not a 7"

It updates the Constitution file for you. One or two refinement rounds after your first few posts is normal.

---

Your voice rules are set. Next: `guide/03-build-your-hook-bank.md`
