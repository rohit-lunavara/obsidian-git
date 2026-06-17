---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> Write a script to pull the latest code from all repos daily—and let Claude Code write it. Al uses a 16-line script (written entirely by Claude Code) that pulls the latest main branch from all 15 repositories every morning. This ensures that he’s always querying current code instead of outdated information, solving the “docs are stale” problem that plagues most technical support teams.
> 
> Maintain a “customer quirks” page to make AI answers customer-specific. Al keeps a Confluence page listing each enterprise customer’s unique deployment requirements: how they handle secrets, namespaces, encryption, air-gapped environments. His Claude Code custom commands reference this page first, generating highly tailored deployment instructions instead of generic answers anyone could Google.
> 
> Combine code repositories with Confluence MCP for maximum context. Al’s custom Claude Code commands first check Confluence for deployment documentation, then query the code repositories if needed. This multi-source approach means Claude Code pulls from official docs, tribal knowledge, and actual implementation—delivering answers no single source could provide.
> 
> Your code is better documentation than your docs. Al realized public documentation couldn’t answer his enterprise customers’ detailed technical questions. By pulling all 15 of Galileo’s repositories into VS Code and querying them with Claude Code, he can now answer questions about how services cascade together, how features actually work, and deployment specifics that aren’t captured anywhere else.
> 
> Turn Slack support threads into knowledge base articles automatically. Using Pylon, Al converts detailed customer conversations into abstracted help articles with one click. These articles are more in-depth and current than official docs because they’re based on real customer questions and don’t require the overhead of PR reviews and approval processes.
> 
> Reduce engineering interruptions to near-zero by self-serving answers. Before this system, Al constantly pinged engineering with customer questions, creating frustration on both sides. Now he queries the code directly, only reaching out to validate answers or when Claude Code can’t find information (usually because it exists only in meeting notes or hallway conversations).
> 
> The human value-add is making AI answers sound human, and knowing when to validate. Al doesn’t blindly copy-paste Claude Code responses. He proofreads everything, removes telltale AI phrases like “in summary,” condenses verbose answers to what customers actually need, and validates complex technical answers with engineering when he doesn’t fully understand the implementation.
> 
> Compete on customer experience, not just product velocity. Everyone uses AI to ship faster products. Al uses AI to show up differently in customer relationships—delivering custom deployment documentation that accounts for each customer’s specific security requirements and infrastructure constraints. This differentiation in service quality is harder to replicate than product features.

https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-i-gave-claude?utm_source=post-email-title&publication_id=10845&post_id=192896152&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true