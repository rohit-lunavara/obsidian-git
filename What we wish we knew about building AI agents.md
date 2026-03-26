---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> 1. Instead of building a full blown AI agent, build an MCP server first since they will help validate demand for further agentic capabilities
> 2. Your harness is not your moat
> 	1. If we were restarting today, we would have skipped building a custom harness and made MCP the canonical interface
> 		1. Using subagents leads to a black box problem as the coordinator couldn’t see what sub-agents were doing leading to context loss and confusion
> 		2. Agent loop with modes and tools is not scalable since custom tools need to be written to make it work within the loop
> 		3. Current harness uses Claude Agent SDK with MCP tools and skills
> 3. Your context is your advantage
> 	1. The combination of your app’s functionality and user data create a unique blend no other product can match
> 	2. You can use the following:
> 		1. MCP Tools - Capabilities selected and extracted from the API
> 		2. Skills - MD files to teach the agent complete workflows and product knowledge
> 		3. Layered runtime context injection - User's current view and state to reduce bloat in the prompt
> 		4. Taxonomy tool - Lets the agent explore user's data on demand rather than stuffing it in the prompt
> 		5. Memory onboarding flow - Collects company and product context through conversation and persists it across sessions, so each user's setup is learnt by the agent over time
> 4. Setup observability and evals from day one
> 	1. AI is non-deterministic and can fail unpredictably
> 	2. We need:
> 		1. Tracing - Input, output, latency, cost
> 		2. Trace IDs
> 		3. Replay and debug specific interactions
> 		4. Curated datasets of real user queries
> 		5. Automated scoring - LLM as judge and deterministic checks
> 5. Always keep the user needs at the forefront

https://newsletter.posthog.com/p/what-we-wish-we-knew-before-building?utm_source=tldrfounders