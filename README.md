# AI LinkedIn Workflow

From idea to published LinkedIn post in 30 minutes.

## What This Is

A system that helps you produce voice-consistent LinkedIn posts using AI. It gives the AI your voice rules, proven post structures, and your actual writing patterns — so the output sounds like you, not like a robot.

**There's no code in here.** This is a folder of text files — voice rules, post frameworks, and instructions that tell an AI how to write like you. You don't need to be technical to use it. If you can open a terminal and type three words, you're good.

The reason it's a repo instead of a regular app is simple: desktop AI tools hide your instructions and memory behind settings screens you can't see or control. Here, everything is in plain text files you can read, edit, and understand. Your voice rules, your past posts, your strategy — it's all visible and yours.

**Why not just prompt ChatGPT?**

You can. And it works for a while. But you'll notice the posts start sounding generic — same sentence structures, same filler phrases, same "Here's the kicker" energy. This system solves that by giving the AI three things a single prompt can't:

1. **Voice rules** — what to avoid (AI cliches) and what to protect (your distinctive patterns)
2. **Proven structures** — frameworks that work on LinkedIn, not just "write a post about X"
3. **Memory** — your past posts, hooks, and strategy so each post builds on the last

Think of it like having a strategist, writer, and editor instead of asking one person to do all three.

**Important: the AI does the work.** When the guides below describe things like "build your hook bank" or "define your voice," that doesn't mean you sit there editing files. You talk to Claude Code, and it handles the file creation, analysis, and organization. Your job is to provide the raw material (writing samples, topic ideas, feedback) and make decisions. Claude Code does the rest.

## Quick Start (Claude Code)

```bash
git clone https://github.com/Optiminz/ai-linkedin-workflow.git
cd ai-linkedin-workflow
claude
```

That's it. Claude Code detects it's your first run and walks you through everything:
1. You paste 2-3 writing samples — it analyzes your voice and saves a profile (5 min)
2. It sets up your voice rules automatically
3. You pick a topic — it develops your first post with hook options and framework suggestions (20 min)
4. You get a publishable post saved to `posts/`, ready to copy into LinkedIn

You talk. It builds. You approve.

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

The `guide/` folder explains what each layer of the system does and why it matters. If you're using Claude Code, you don't need to follow these as manual instructions — Claude Code handles the setup and file management. The guides are there so you understand what's happening and can make better decisions about your content.

| Step | What It Covers | When It Becomes Relevant |
|------|---------------|------------------------|
| 01 | Your first post | Day 1 |
| 02 | How voice rules work | After 2-3 posts, "doesn't sound like me" |
| 03 | How the hook bank works | Curious why the hooks keep improving |
| 04 | How post tracking works | After ~5 posts, want to see patterns |
| 05 | How voice samples deepen your profile | Voice still not quite right |
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

This is essentially the same system used internally at [Optimi](https://optimi.co.nz) for client content — the production version also integrates with Notion for editorial calendars and a vector database for long-term voice memory across hundreds of posts. This repo is the standalone core that works without any external services.

## License

MIT
