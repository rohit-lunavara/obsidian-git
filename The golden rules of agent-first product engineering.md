---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> ![[Pasted image 20260511200018.png]]
> 
> you need to build for agents as a _primary_ surface, not an afterthought
> 
> Golden rules:
> 
> Let agents do everything users can do
> 	Deliberate exceptions for situations where requiring human input makes sense
> 	Nearly everything in your API needs to be accessible to agents
>    
> Meet agents at their level of abstraction
> 	The more "raw" your product's agent interface is, the more creative potential you can unlock
> 	For example, let agents query data using SQL instead of making get/read endpoints for each resource
> 
> Front-load universal context
> 	Since you're building an agent experience for your specific product, the problem space is much smaller - you already know the key scenarios, tools and use cases
> 
> Writing skills is a human skill
> 	Agent skills close the gap between what your product can do and what an agent can do out of the box with your tools
> 	Skills should only contain context that a human can provide since an agent can't discover by itself
> 		Idiosyncratic knowledge, edge cases, taste and craft
> 
> Treat agents like real users
> 	Dogfooding headlessly - Use the CLI over the UI since that is the same env as the agent
> 	Doing manual trace reviews - Go through real user sessions that have user feedback ratings
> 	Feeding our intuition into a loop - Build evals based on what you catch - both good and bad

https://newsletter.posthog.com/p/the-golden-rules-of-agent-first-product?utm_source=post-email-title&publication_id=1318225&post_id=193549431&utm_campaign=email-post-title&isFreemail=true&r=969sr&triedRedirect=true