---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> A loop is just a prompt that fires itself, nothing more exotic than that. The reason “loops” sound intimidating is that the hype cycle turned a basic automation concept into something mystical. Heartbeats, crons, and webhooks have been around forever. What’s new is pointing them at an AI agent instead of a batch job.
> 
> Goals are the most powerful loop type, and the one most people get wrong. A goal loop sets an outcome and runs an agent against it until the outcome is validated or the agent gets stuck. It doesn’t stop on a timer; it stops when the work is actually done. Fuzzy success criteria means the agent loops forever, burning tokens, so my advice is to let Codex write its own goals, using OpenAI’s goal-writing guide as a starting point.
> 
> Think about loops the way you think about onboarding an employee. Define the job: what they check, how often, what output you want, and who to contact when something’s wrong. “Every Friday at 10 a.m., review all merged PRs and identify skills our agents are missing” is a job description. It’s also a loop prompt.
> 
> Your agent can have its own agents. This is where loops get truly powerful. The PR-review loop Claire built in Claude Code doesn’t just check PR status; it spins off dedicated subagents to babysit individual PRs until all merge checks are green. The skills loop in Codex identifies gaps and immediately spawns subagents to validate each new skill using a goal loop.
> 
> Loops get expensive if you don’t write them carefully. If the success criteria is vague or the validation threshold is too thin, the agent will keep running and keep charging without meaningful progress. Monitor both cost and output quality from day one.
> 
> The morning briefing in Claude Cowork is a perfect loop starter. A scheduled task that fires every morning, checks your calendar and email, and sends a summary to Slack is already a fully functional loop. No code required. From there, scaling up to PR reviews or skills identification in Claude Code or Codex is a natural next step.
> 
> The power move is loops that generate their own subagent loops. In the Codex demo, Claire’s weekly automation spawned two named subagents that each ran their own goal loops to validate skills in real time. The ceiling on loop-based automation is basically “how well can you define the job?” not “how complex is the engineering?”

https://www.lennysnewsletter.com/p/how-i-ai-how-to-write-ai-agent-loops?utm_source=post-email-title&publication_id=10845&post_id=202479892&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true