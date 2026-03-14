---
title: 'Scaffolding is Tech Debt'
description: "If you're spending more time tuning your AI workflow than clarifying what you're building, you might be investing in the wrong layer."
pubDate: '2026-03-14'
heroImage: '../../assets/scaffolding-is-tech-debt.jpeg'
---

Every few weeks someone shares their elaborate AI coding setup. Custom prompts chained together. Wrapper scripts. Carefully tuned system instructions. Hours of work making the current model do something it almost can do.

Then a new model drops and half of it stops working. Or worse — it still works, but the model can now do it natively, so all that scaffolding is just getting in the way.

I've done this myself. Spent time crafting the perfect prompt chain for a task, felt clever about it, then watched the next update make it unnecessary. There's a name for this pattern, and it comes from a completely different corner of AI.

In 2019, AI researcher Richard Sutton wrote an [800-word essay](http://www.incompleteideas.net/IncIdeas/BitterLesson.html) called "The Bitter Lesson." His observation: researchers repeatedly tried to inject human domain knowledge into AI systems, believing their expertise would make the models smarter. Every time, the approach that won was simpler — just make the model bigger, give it more data. Scale beat cleverness, consistently.

I have a printed copy on my desk. Boris Cherny, the creator of Claude Code at Anthropic, keeps a framed copy on the wall. It's that kind of essay — short enough to read in five minutes, important enough to keep where you can see it.

The bitter lesson was written about AI research, but it applies perfectly to how we use AI tools. Every elaborate workaround we build for a model's current limitations is the same mistake Sutton warned about: betting on human cleverness over scale. The next model will handle it natively. Your scaffolding becomes tech debt overnight.

Boris puts it bluntly: "Never bet against the model. Scaffolding you build to extend capability by 10-20% will be wiped out by the next model."

Every workaround you build now has a shrinking shelf life.

Here's a practical example. You don't need to run `/init` on your projects. You don't need an elaborate CLAUDE.md, COPILOT.md, or AGENTS.md. The model can read your `package.json`. It can figure out your directory structure. It can work out your test command. Most of what people put in these files is information the agent can already discover and auto-generated context files actually *reduce* task success while increasing cost. You're adding noise.

What belongs in those files is genuinely non-discoverable information: "we use this unusual deploy pipeline," "don't mock the database in integration tests," "this service talks to that legacy API via this specific auth flow." Twenty lines, tops. Anything more and you're probably writing scaffolding.

And even the useful bits need regular pruning. I review my global instructions file periodically and delete anything the model has gotten better at handling on its own. Boris Cherny's CLAUDE.md for Claude Code itself is two lines long. His advice: delete yours and start fresh. Each new model needs less hand-holding. I've published a [Claude Code skill](https://github.com/dariatrainor/claude-skills/blob/master/skills/audit-claude-md/SKILL.md) that audits your CLAUDE.md and classifies each instruction as foundation or scaffolding — try it on yours and see how much you can cut.

So if most of what we build around AI tools is temporary, what actually compounds? Clear specifications. Good test suites. Well-structured codebases. The prompt that gets your current model to handle edge cases correctly — that's scaffolding. The acceptance criteria that define what "correct" actually means — that's foundation. One has a shelf life of weeks. The other compounds over time.

If you're spending more time tuning your AI workflow than clarifying what you're actually trying to build, you might be investing in the wrong layer.