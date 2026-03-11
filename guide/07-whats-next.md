# Guide 07: What's Next

**Where you are:** You've got the core system running. This guide covers advanced features, the bigger picture, and where to go from here.

---

## Lakajev conversion scoring

Getting likes is easy. Getting someone to reach out is the actual goal.

The Lakajev score is a conversion quality check built into `/lidev` as an optional step. Before you finalize a post, it asks: what's the chance this generates an inbound message versus just approval from existing followers?

It evaluates three things:

- **Gift:** Does the post give something genuinely useful — a framework, a perspective, a process — rather than just a take?
- **Step-through:** Does it walk through the reasoning, not just state the conclusion? People trust what they can follow.
- **Language match:** Does it use the words your target audience uses to describe their problems, not the words you use internally?

A post can score high on voice and low on conversion. That's useful to know before publishing. Run it when you care about leads, skip it when you're posting for other reasons.

---

## Adding your own frameworks

The `frameworks/` folder holds reusable post structures — patterns that work across different topics. The system comes with some. You can add your own.

When you see a post structure you want to repeat:

1. Write out the skeleton: what's the opening move, how does it develop, how does it close?
2. Note what makes it work — what tension it creates, what it assumes the reader already believes
3. Save it to `frameworks/your-framework-name.md`

Keep it abstract enough to reuse. "Lead with the counterintuitive claim, then show the mechanism, then give one concrete example" is a framework. A specific post about pricing is not.

---

## Quality check: the read-aloud test

Before publishing anything, read it aloud. Not in your head — out loud.

If you stumble on a phrase, cut it or rewrite it. If a sentence makes you sound like you're presenting at a conference when you're talking to someone one-on-one, simplify it. If you'd never say it in conversation, it probably shouldn't be in a LinkedIn post.

This catches more than voice scoring algorithms. Your ear knows before your editor does.

---

## The full writing workflow

This system is scoped to LinkedIn. For longer-form content — newsletters, blog posts, whitepapers — there's a separate production system built on the same principles but designed for the longer arc: research, structure, multiple drafts, quality gates.

It's called [ai-writing-workflow](https://github.com/Optiminz/ai-writing-workflow). Seven specialized personas, a critic that scores 0–100 before anything publishes, and a system learning layer that updates the constitution when something fails.

Worth looking at if you're writing long-form regularly and want the same level of voice consistency across both formats.

---

## Contributing

If you've built something worth sharing — a framework that works, a hook structure that converts, a fix for something that broke — GitHub issues are the right place.

Framework submissions: open an issue with the structure and an example post that used it. If it's solid, it goes into the repo for everyone.

Bug reports, suggestions, and improvements all welcome. The system gets better when people who use it share what they find.

---

That's the guide. The rest is practice.
