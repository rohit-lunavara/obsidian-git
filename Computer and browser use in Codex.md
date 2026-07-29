---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> 
> AI testing can be far more exhaustive than human testing. When Claire tests her own onboarding flow, she naturally follows the happy path. She fills out every required field, clicks “next,” and never intentionally tries to break anything. Codex tested the flow as both a team and an individual, pushed on required-field edge cases, and immediately uncovered a blocking bug that had survived for months simply because Claire always completed the form correctly.
> 
> Frontier models often perform better when they are given room to think. When Claire first started using browser use, she would give the model a list of 25 things to test. Now she simply says, “QA the onboarding flow,” and lets it decide how to approach the task. The result is often broader coverage, with fewer blind spots introduced by her own assumptions about what matters.
> 
> Persona testing with browser use can reveal friction that synthetic user research misses. Claire’s husband, EJ, came up with the idea. Rather than asking AI to evaluate a product in the abstract, he suggested having it use the product as a specific person: a PM coming out of a meeting, an engineer picking up a PRD, or a team lead checking usage. In ChatPRD, this approach exposed a structural problem in the cross-thread reference flow. Claire already knew the issue existed, but she had never experienced it so clearly from the user’s perspective.
> 
> LinkedIn browser use is genuinely useful, but Claire initially used far more compute than the task required. She started by running the workflow on GPT-5.6 at high effort. After dropping to a medium-effort model, it could still work through unread messages, draft context-aware replies, and flag anything that needed a personal response. For anyone sitting on hundreds of LinkedIn messages without an official MCP or API connection, browser use is a practical solution.
> 
> Computer use can even operate an iPhone through screen mirroring. Claire was traveling out of state while the software she needed to manage her home Wi-Fi was installed on a phone back in California. She needed to open firewall ports so she could SSH into her Mac Minis remotely. Codex opened iPhone mirroring, updated the router settings, completed the SSH setup, and closed the ports again when it was finished. That would have been nearly impossible for her to do manually from a hotel room.
> 
> The model and effort level should match the job. Sorting through LinkedIn messages requires a very different level of reasoning than writing production code or conducting an exhaustive QA pass. Choosing the right amount of compute makes these workflows faster and cheaper. That becomes especially important when browser use is running throughout the day.
> 
> When a website blocks the agent, the human can step in briefly. During a Free People shopping session, the site flagged Codex as a bot and presented a CAPTCHA. Claire completed the verification, then handed control back. It is a useful division of labor: AI handles the tedious browsing and filtering, while the human takes care of the moments that require verified identity.

https://www.lennysnewsletter.com/p/how-i-ai-claude-opus-5-review-browser?utm_source=post-email-title&publication_id=10845&post_id=207971942&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true