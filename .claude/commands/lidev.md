---
description: Develop a LinkedIn post using systematic frameworks. Use when the user requests LinkedIn content development or invokes /lidev. Handles topic clarification, framework selection, hook development, collaborative refinement, quality assessment, and final delivery in a code block ready for copying.
argument-hint: topic or idea to develop (e.g., "why most software rollouts fail" or "the hidden cost of bad data")
---

# LinkedIn Post Development

You are developing a high-quality LinkedIn post. Your job is to collaborate on post development — not to auto-generate a finished draft on the first pass. Work through each step with the user.

---

## Step 0: Load Context

Before doing anything else, read these files:

1. **Constitution:** `EDITORIAL-CONSTITUTION.md`
   - Voice dimensions, AI Tells list, Keep List patterns
   - This governs every word in the final post

2. **Voice samples:** `voice-samples/`
   - Read examples to calibrate tone before drafting
   - Reference these during the drafting step

3. **Hook bank:** `hook-bank.md`
   - Check for unused hooks that fit the topic before generating new ones
   - A strong existing hook should be preferred over generating fresh ones

4. **Post log:** `post-log.md`
   - Scan the last 5 entries to avoid repeating recent topics, angles, or structures

5. **Frameworks:** `frameworks/README.md`
   - Available content frameworks and when to use each

---

## Step 1: Topic Clarification

If the topic provided is vague or underdeveloped, ask 1-3 clarifying questions before proceeding. Do not draft anything yet.

Good clarifying questions:
- "What's the core observation or tension here — what's wrong with how most people approach this?"
- "Do you have a real example or result you want to anchor this in?"
- "Who is this aimed at — what would they be feeling when this post lands in their feed?"
- "Is this meant to generate conversation, attract a specific type of person, or demonstrate expertise?"

Only proceed to Step 2 once you understand the angle clearly enough to suggest frameworks.

---

## Step 2: Framework Selection

Suggest 2-3 framework options with rationale for why each fits this topic. Do not auto-pick — present the options and let the user choose.

Available frameworks are in `frameworks/README.md`. Common ones:

**Contrarian Authority Pattern**
Best for: Challenging conventional wisdom. Works when there's a widely-held belief you can credibly flip.
Structure: State what most people do → why it fails → what actually works

**Rule of 3 Pattern**
Best for: Frameworks, lists, lessons. Works when the insight has natural structure.
Structure: Hook → 3 parallel points → takeaway or CTA

**Upgraded Playbook Pattern**
Best for: Positioning a better methodology. Works when you have a systematic approach to contrast against a common one.
Structure: Old way → problem with old way → new approach → how to apply

**Story Arc Pattern**
Best for: Practitioner credibility. Works when there's a before/after with a clear turning point.
Structure: Before state → pivotal moment → after state → transferable lesson

**Diagnostic Pattern**
Best for: Attracting ideal clients. Works when you can identify a specific symptom their target reader would recognize.
Structure: Symptom → what it usually indicates → the actual fix

State your recommended frameworks with rationale:
- Framework 1: [name] — [why it fits this topic]
- Framework 2: [name] — [why it fits this topic]
- Framework 3 (optional): [name] — [why it fits this topic]

Wait for the user to choose before proceeding.

---

## Step 3: Hook Development

Check `hook-bank.md` for unused hooks matching this topic or theme. If a strong match exists, surface it as Option 1 with a note that it came from the bank.

Then provide 3 hook options with rationale. For each, flag whether the **protagonist is the READER or the AUTHOR** — reader-centered hooks perform better and should be presented first.

Format:
- **Option 1:** [Hook text] — [rationale] — Protagonist: Reader ✅ / Author ⚠️
- **Option 2:** [Hook text] — [rationale] — Protagonist: Reader ✅ / Author ⚠️
- **Option 3:** [Hook text] — [rationale] — Protagonist: Reader ✅ / Author ⚠️

Hook quality standards:
- Opens within 3 mobile lines (roughly 200 characters before "...see more")
- Does not open with "I" as the first word
- Creates tension, curiosity, or recognition — not a thesis statement
- No clickbait — the post must deliver on what the hook implies
- No forbidden phrases (see Constitution)

After the user picks a hook: save the unused options to `hook-bank.md` with date, theme, hook text, why not chosen, and reuse potential.

---

## Step 4: Full Draft

Using the chosen framework and hook, write the full post.

**Structure:**
1. Hook — the chosen hook from Step 3
2. Context — brief situation, observation, or market reality (1-2 sentences)
3. Core content — the framework, insight, story, or lesson (3-5 short paragraphs or structured points)
4. Application — how the reader can use or evaluate this (1-2 sentences)
5. Engagement close — a question or soft CTA that invites response

**Voice enforcement (check against Constitution before presenting):**

_Formatting:_
- No markdown symbols in post text — no **, __, ##, or similar
- Use • for bullet points if needed, numbers for sequential steps
- 2-4 emojis maximum, placed for emphasis not decoration
- Mobile-optimized: first line must land within 3 lines before "...see more"

_AI Tells:_
- Scan the draft against the AI Tells list in the Constitution
- Remove any flagged words or phrases before presenting
- This is non-negotiable — do not present a draft with known AI Tells

_Keep List:_
- Check that distinctive voice patterns from the Keep List survive
- Do not smooth them out in the name of clarity

_Engagement close patterns — rotate through:_
- Direct question to reader: "Which of these does your [team/operation/firm] struggle with most?"
- Soft DM invite: "Drop me a message if you want to work through this."
- Open observation: "Curious what others have seen here."
- Inclusive pull: "Anyone else running into this?"
- Combined: question + DM invite for higher conversion potential

_Engagement close — forbidden (overused):_
- "For anyone passing by here..."
- "For anyone following along..."

---

## Step 5: Collaborative Refinement

After presenting the draft, run the pre-flight checks and share results before asking for feedback.

**Check 1 — Protagonist (mandatory)**
Who is the subject of line 1 — the reader or the author?
- Reader: "You've just approved the platform budget..." ✅
- Author: "The most useful question I've asked..." ⚠️ flag for revision

**Check 2 — AI Tells scan (mandatory)**
Scan the post against the Constitution's AI Tells list.
- Any matches: flag and revise before presenting
- Present clean or note what was removed

**Check 3 — Voice integrity (mandatory)**
Does the post sound like the voice samples? Apply the byline test:
- Could this post be signed by a generic thought leader or a consultant firm? ⚠️ too generic
- Could only this specific author have written it? ✅

**Check 4 — Proof and specificity**
Is there a stated outcome, named tool, or specific scenario grounding the post?
- Named and specific = ✅
- "A client told me..." or "Many companies..." = ⚠️ flag as vague

After sharing check results, ask: "What would you like to change?"

Refine until the user confirms they're happy with the post.

---

## Step 6: Optional Conversion Score

If the user wants a conversion quality check, run the Lakajev framework assessment.

This measures whether the post will generate an inbound inquiry — a post can be well-crafted and still score low here.

**Window Test (0-60 pts)**

_Reflection (0-20):_ Does a reader in your target audience see themselves in line 1?
- Nouns from their world, their role, their problem = high score
- Author-centered hook = max 10/20

_Gift (0-20):_ Once they click "see more," is there a concrete payoff?
- Framework, diagnostic, belief flip, "finally someone gets it" moment = high score
- Vague inspiration or generic insight = low score

_Step-Through (0-10):_ Does the post give a next action that moves toward working with you?
- DM prompt, profile visit, direct contact = high score
- War story question only = max 4/10

_Present Test (0-10):_ If they visit your profile after reading, will they find more for them?
- Post clearly signals who you help = high score
- So generic a visitor can't tell who you serve = low score

**Language Match (0-20 pts)**
Score across 5 layers:
- Functional: Uses verbs from their daily work, not consultant-speak
- Technical: Uses insider vocabulary they'd recognize
- Cultural: References shared experiences from their world
- Psychic: Voices their internal monologue ("what if this goes wrong")
- Narrative: Describes their repeating story loop

**Carrier Trust (0-20 pts)**
- Lived Credibility: Author sounds like they've done this, not just studied it
- Proof Proximity: Result attributed to someone like the reader
- Motive Transparency: Why is this being shared? Does it imply what you do?
- Values Polarity: Does this attract the right person and gently repel the wrong one?

**Thresholds:**
| Score | Action |
|-------|--------|
| 80+ | Strong for conversion — deliver |
| 60-79 | Identify weakest dimension and revise |
| Below 60 | Rebuild with reader-centered approach |

---

## Step 7: Final Delivery

Present the approved post in a code block for easy copying:

```
[post text here]
```

Flag any claims that need verification before posting (e.g., statistics, attributed outcomes).

---

## Step 8: Save Post File

Write the post to `posts/YYYY-MM-DD-[slug].md` with this metadata header:

```markdown
---
date: YYYY-MM-DD
topic: [one-line description]
framework: [framework used]
hook: [which hook option was chosen]
status: draft
linkedin_url:
---

[post text]
```

Confirm the file path when done.

---

## Step 9: Hook Bank Update

Offer to save unused hooks to `hook-bank.md`.

Format for each entry:
```
## [Date] — [Theme]
**Hook:** [hook text]
**Why not chosen:** [brief reason]
**Reuse potential:** [high/medium/low] — [when it might work]
```

---

## Step 10: Publish Tracking

After the post goes live, the user can paste the LinkedIn URL to update `post-log.md`.

Format for post-log entry:
```
| YYYY-MM-DD | [topic] | [framework] | [LinkedIn URL] | [engagement notes] |
```

Remind the user: "Paste the LinkedIn URL when it's published and I'll update the post log."

---

## Quality Assessment Rubric

Run this internally before delivering the draft. Target: 85+/100.

**Voice & Authenticity (25 pts)**
- Matches the voice dimensions from the Constitution (5)
- Avoids overly dramatic or hyperbolic language (5)
- Professional but approachable — sounds human (5)
- Demonstrates systematic or analytical thinking (5)
- Claims are evidence-based, not fabricated (5)

**Content Philosophy (25 pts)**
- Shows results of actual work, not just opinion ("sawdust method") (5)
- Reveals the real problem, not the surface-level version (5)
- Focused on the reader's needs, not the author's resume (5)
- Moves from broad to specific — "crowded room to table for two" (5)
- Demonstrates a unique mechanism, framework, or perspective (5)

**Strategic Positioning (25 pts)**
- Reinforces a clear positioning or point of view (5)
- Relevant to the intended target audience (5)
- Demonstrates expertise without fabrication or puffery (5)
- Differentiates from generic content on the same topic (5)
- Builds credibility in a specific domain (5)

**LinkedIn Format & Structure (25 pts)**
- Follows formatting standards — no markdown symbols (10)
- Engagement close is fresh and appropriate (5)
- Mobile-optimized opening (5)
- Readable without scrolling through walls of text (5)

---

Topic or idea to develop: $ARGUMENTS
