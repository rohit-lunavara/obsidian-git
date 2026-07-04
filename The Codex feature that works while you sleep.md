---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> 
> Goals enable AI to work autonomously for hours without supervision. Claire ran a goal in Codex that worked for five hours and 45 minutes—the longest she’s ever had an AI agent run successfully. Unlike standard prompts that require turn-by-turn interaction, Goals create a loop where the AI works, verifies, checks, and continues until it hits the defined outcome.
> 
> The difference between a prompt and a Goal is fundamental. A prompt is an instruction of what to do (“Rewrite this code”). A Goal is a description of what a good outcome looks like and how to get there (“Reduce P95 checkout latency below a defined threshold while keeping the correctness suite green”).
> 
> Claire eliminated hundreds of error logs by pointing Goals at her Sentry data. She gave Codex access to every trace of invalid operations, then set a goal: categorize each issue, fix it, then replay all historical examples until every error is solved. The result: zero errors remaining, and instead of bandaid fixes scattered throughout the code, she got a systematic, intelligent framework.
> 
> Goals work incredibly well for non-technical tasks. Claire cleaned 3,900 emails down to 68 in under four hours by setting a simple goal: categorize all emails, unsubscribe from unnecessary ones, and clean up the inbox. The AI read every email, created labels, clicked unsubscribe links, and left her with only the emails requiring judgment.
> 
> Strong Goals have six key components: outcome (what should be true when done), verification (how to test it), constraints (what can’t regress), boundaries (what tools and files to use), iteration policy (how to decide what to try next), and stopping conditions (when to ask for help). Product managers who’ve written good OKRs will recognize this framework immediately.
> 
> Working with Goals feels like managing a colleague, not babysitting a tool. You assign a task, the AI goes away for the time required (whether that’s 30 minutes or five hours), and comes back with completed work for you to review. Claire found herself “twiddling her thumbs” because so much of the work was now handled autonomously.
> 
> Goals aren’t token-cheap, but they’re worth it. Claire’s email cleanup used about 6 million tokens over four hours. But the alternative—manually categorizing thousands of emails or chasing down hundreds of error logs—would take far longer and be far more tedious.

https://www.lennysnewsletter.com/p/how-i-ai-codex-goals-explained-and?utm_source=post-email-title&publication_id=10845&post_id=199541302&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true