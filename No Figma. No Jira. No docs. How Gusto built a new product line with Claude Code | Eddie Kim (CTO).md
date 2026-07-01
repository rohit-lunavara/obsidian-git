---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> 
> A five-person team with no process can outship a large team with full process, if AI handles the engineering. Eddie’s product launched at Gusto’s tier-one level after 10 weeks, starting from zero code. The constraint wasn’t a liability—it was the design. When AI does the building, coordination overhead doesn’t scale the engineering; it just slows it down. The key: strip process to what the team actually needs, then let AI fill the gap.
> 
> “Zero code to tier-one launch” is now a viable founding path. The team reached a production milestone at Gusto without a line of pre-existing code. This flips the assumption that early teams spend months on infrastructure before shipping anything real. With Claude Code as the primary builder, the initial sprint becomes about direction and judgment, not typing. It compresses the time between idea validation and real user contact from months to weeks.
> 
> No meetings, no Jira, no text threads. It shipped anyway. The team had no standup cadence, no ticket system, no async thread to resolve blockers. What replaced all of that: shared context held inside the AI loop. When the model carries state and the team is small and aligned, human coordination overhead becomes optional.
> 
> The technical stack for a production AI agent is shockingly minimal. The entire agent loop ran on Cloudflare Workers with the Vercel AI SDK. Nothing else. No proprietary orchestration layer, no third-party agent framework. Everything else was built in-house. Teams often over-architect before they’ve proven anything; Eddie’s stack is evidence that infrastructure minimalism accelerates the path to learning what the agent actually needs to do.
> 
> Building agents is not as complicated as the community makes it sound. An agent is an AI SDK running somewhere in the cloud, able to look up files and call tools. That’s the full definition. The complexity people fear (state management, orchestration, reliability) is solvable with the same judgment calls any backend system requires. Eddie’s team shipped one at production quality in 10 weeks without specialist AI infrastructure experience.
> 
> The “permanent Zoom” model of AI development changes how teams think about context. Claude Code running in a persistent loop means the model has continuous access to the codebase’s current state. That’s closer to having an engineer who never closes their laptop than a chat interface you query on demand. For small teams, this is the equivalent of a senior engineer who is always available, always current, and never needs onboarding after a break.
> 
> The lesson for founding teams isn’t “use Claude Code.” It’s “design your process for AI as a team member.” Most early teams graft AI tools onto a human-scaled workflow: standups, tickets, PRs reviewed by three people. Eddie’s team treated the AI as a primary contributor from day one and built their coordination model around that assumption. The result: a workflow that gets faster as the AI improves, not one that merely offloads tasks to it.

https://www.lennysnewsletter.com/p/how-i-ai-glm-52-review-and-how-gusto?utm_source=post-email-title&publication_id=10845&post_id=203730644&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true