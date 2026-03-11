# AI LinkedIn Workflow — Claude Code Configuration

This file tells Claude Code how to work in this repo. Read it once per session.

---

## First Run Detection

**Check these two conditions at the start of every session:**

1. Does `voice-samples/` exist and contain any `.md` files outside `voice-samples/examples/`?
2. Does `EDITORIAL-CONSTITUTION.md` exist and contain no `[PLACEHOLDER]` values?

**If either check fails — this is a new setup.** Run the welcome flow below before anything else.

---

### Welcome Flow (New Setup)

Run this once when the user first opens the repo. Target: 30 minutes total.

**Step 1 — Welcome (2 min)**

Tell the user:

> "Welcome to AI LinkedIn Workflow. Here's what this system does:
>
> You give it your voice — writing samples, phrases you like, things you want to avoid. It stores those rules in files it can read every session. When you write a post, it pulls in your voice rules, proven post structures, and your past hooks so the output sounds like you, not like a robot.
>
> To get started, I need 2-3 pieces of your actual writing. These can be LinkedIn posts, emails, blog excerpts, Slack messages — anything you wrote that sounds like you at your best. Paste them below."

**Step 2 — Voice Capture (5 min)**

When the user pastes their samples:

1. Read all samples carefully
2. Identify 4-6 patterns across these dimensions:
   - Sentence rhythm (short punchy vs long flowing vs mixed)
   - Opener style (observation, question, statement, story)
   - How they handle specificity (named tools/people vs general)
   - Phrases or constructions that recur
   - Tone (how serious vs playful, formal vs casual)
   - What they DON'T do (absent patterns worth protecting against AI defaults)
3. Summarize findings back to the user in plain language before saving

**Step 3 — Save Voice Analysis (2 min)**

Create `voice-samples/` directory if it doesn't exist. Save analysis to `voice-samples/[first-name].md` using this structure:

```markdown
# [Name]'s Voice Profile

## Captured [Date]
Source samples: [brief description]

## Patterns

### Sentence Rhythm
[what you found]

### Opener Style
[what you found]

### Specificity
[what you found]

### Recurring Phrases or Constructions
[list them]

### Tone
[what you found]

### What to Protect (distinctive patterns AI tends to smooth away)
[list them]

## AI Tells to Avoid
[phrases or patterns that appeared in AI suggestions but not in their writing]
```

**Step 4 — Initialize Constitution (2 min)**

If `EDITORIAL-CONSTITUTION.md` doesn't exist, create it from `templates/constitution-template.md` if that exists, or create a minimal version:

```markdown
# Editorial Constitution

## Voice Rules

### AI Tells (Never Use)
Phrases that don't appear in this writer's natural voice:
- [populate from voice analysis]

### Keep List (Protect These)
Distinctive patterns to preserve even when they feel unconventional:
- [populate from voice analysis]

## Tone Target
[intensity level, formal/casual balance — from voice analysis]

## Formatting Rules
- No bold/italic markdown in LinkedIn posts (** and __ don't render on LinkedIn)
- Clean text, use • for lists, numbers for sequential steps
- Final post always in a code block for easy copying
- Strategic emoji: 2–4 max per post
```

**Step 5 — First Post (20 min)**

Immediately transition to `/lidev` — don't end the session here. Say:

> "Voice profile saved. Let's use it right now and write your first post. What's a topic you've been meaning to write about, or something that happened recently that would make a good LinkedIn post?"

Then run the lidev flow.

---

## Every Session: What to Load

At the start of any session (first run or returning):

1. **`EDITORIAL-CONSTITUTION.md`** — load voice rules, AI Tells, formatting standards
2. **`voice-samples/`** — load all `.md` files (except `examples/`) for pattern matching
3. **`hook-bank.md`** — load if it exists, for suggesting reusable hooks
4. **`idea-bank.md`** — load if it exists, for surfacing parked topics
5. **`post-log.md`** — load if it exists, to avoid repeating recent topics

If any of these files don't exist yet, note it quietly and continue — don't block on missing optional files.

---

## Skills

**`/lidev`** — Core post development skill

Located at `.claude/commands/lidev.md`. This is the primary workflow. Runs when the user types `/lidev` or describes wanting to write a post.

What it does:
- Takes a topic or angle
- Suggests 3 hook options with rationale
- Collaborates on refinement
- Applies frameworks from `frameworks/`
- Delivers final post in a code block
- Saves to `posts/YYYY-MM-DD-[slug].md`
- Offers to update `post-log.md` after publishing

**`/strategy`** — Content strategy skill

Located at `.claude/commands/strategy.md`. Runs when the user wants to think about content pillars, cadence, or their overall LinkedIn approach.

---

## Post Development Rules

**Voice comes first.** Before generating any post content, check the voice profile and Constitution. If a phrase feels off — generic, AI-sounding, too smooth — flag it and revise.

**Framework options, not prescriptions.** Offer frameworks from `frameworks/` as options, not requirements. Some posts don't need a named structure.

**Hooks are the highest-leverage element.** Always generate 3 hook options. Reference `hook-bank.md` for patterns that have worked. A strong hook is specific, creates mild tension or curiosity, and doesn't give away the whole post in the first line.

**Final delivery format:**
- Always present the final post in a code block
- Include character count if close to LinkedIn's 3,000 character limit
- Note any emojis used (easy to adjust)

---

## Formatting Rules (LinkedIn-Specific)

- **No markdown formatting** — LinkedIn doesn't render `**bold**` or `_italic_`. Plain text only.
- **Line breaks** — Short paragraphs with blank lines between. One idea per paragraph.
- **Lists** — Use `•` for bullets, numbers for sequential steps
- **Emoji** — 2–4 per post maximum. Use at natural break points, not as decoration.
- **Length** — Optimal 150–300 words. Up to 3,000 characters maximum.
- **Hook** — First line visible before "see more" click. Make it earn the click.

---

## File Conventions

| File | Purpose |
|------|---------|
| `posts/YYYY-MM-DD-slug.md` | One file per post draft |
| `post-log.md` | Running log of published posts |
| `hook-bank.md` | Reusable opening lines and hook patterns |
| `idea-bank.md` | Topic parking lot |
| `voice-samples/[name].md` | Voice profile (created during setup) |
| `EDITORIAL-CONSTITUTION.md` | Master voice rules document |

---

## What Not to Do

- Don't use "Here's the kicker", "Here's the catch", "Let's dive in", or "Without further ado"
- Don't open with "I" (weak hook)
- Don't write generic advice that could apply to anyone — get specific
- Don't skip the hook options step — the hook is the most important element
- Don't deliver the post outside a code block — the user needs to copy it cleanly
