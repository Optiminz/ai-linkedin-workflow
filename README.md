# AI LinkedIn Workflow

From idea to published LinkedIn post in 30 minutes.

## What This Is

A system that helps you produce voice-consistent LinkedIn posts using AI. It gives the AI your voice rules, proven post structures, and your actual writing patterns — so the output sounds like you, not like a robot.

**Why not just prompt ChatGPT?**

You can. And it works for a while. But you'll notice the posts start sounding generic — same sentence structures, same filler phrases, same "Here's the kicker" energy. This system solves that by giving the AI three things a single prompt can't:

1. **Voice rules** — what to avoid (AI cliches) and what to protect (your distinctive patterns)
2. **Proven structures** — frameworks that work on LinkedIn, not just "write a post about X"
3. **Memory** — your past posts, hooks, and strategy so each post builds on the last

Think of it like having a strategist, writer, and editor instead of asking one person to do all three.

## Quick Start (Claude Code)

```bash
git clone https://github.com/Optiminz/ai-linkedin-workflow.git
cd ai-linkedin-workflow
claude
```

The system detects it's your first run and walks you through:
1. Pasting 2-3 writing samples so it learns your voice (5 min)
2. Writing your first post with framework options and hook development (20 min)
3. A publishable post saved to `posts/`

## Quick Start (Any AI Tool)

```bash
git clone https://github.com/Optiminz/ai-linkedin-workflow.git
```

1. Open `prompts/lidev-standalone.md`
2. Paste your writing samples and topic where indicated
3. Copy the entire prompt into ChatGPT, Claude.ai, or any AI tool
4. Follow the guided flow to produce your post

## What's Inside

```
posts/                    your posts land here
hook-bank.md              reusable opening lines
idea-bank.md              topic parking lot
post-log.md               published post tracker
voice-samples/            writing examples that teach the AI your style
frameworks/               proven post structures (3 included)
prompts/                  standalone prompts for non-Claude-Code users
guide/                    progressive learning guide (7 steps)
EDITORIAL-CONSTITUTION.md your voice rules (template)
CLAUDE.md                 Claude Code configuration
.claude/commands/         skills: /lidev (post dev), /strategy (content strategy)
```

## The Guide

The `guide/` folder has 7 steps you can work through at your own pace. Each one unlocks a new layer of the system:

| Step | What You Get | When You'll Want It |
|------|-------------|-------------------|
| 01 | Your first post | Day 1 |
| 02 | Voice rules (Constitution) | After 2-3 posts, "doesn't sound like me" |
| 03 | Reusable hook collection | Good hooks getting wasted |
| 04 | Post tracking | After ~5 posts, want to see patterns |
| 05 | Deep voice training | Constitution alone isn't enough |
| 06 | Content strategy | After ~10 posts, ready for a system |
| 07 | Advanced features | Want more (scoring, custom frameworks) |

## Tool Compatibility

| Tool | Experience | Notes |
|------|-----------|-------|
| **Claude Code** | Best | Reads files, remembers voice, saves posts, runs skills |
| **Claude Desktop** | Good | Same AI, but can't see file edits in real time |
| **ChatGPT / Claude.ai** | Works | Use standalone prompt, paste more context manually |
| **Cursor / Windsurf** | Good | File access like Claude Code, different skill format |

Claude Code gives the smoothest experience because it reads your voice rules, suggests hooks from your bank, and saves posts automatically. But every core feature works with any AI tool through the standalone prompt.

## Built With

This system was extracted from [ai-writing-workflow](https://github.com/Optiminz/ai-writing-workflow), a production content system battle-tested with 20+ posts. Built by a strategist + AI.

## License

MIT
