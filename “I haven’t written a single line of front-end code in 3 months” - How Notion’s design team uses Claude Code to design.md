---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> 
> Designs are shifting to code-first prototyping. While Brian still spends 60% to 70% of his time in Figma, he believes designers increasingly need to understand what AI models can actually do. This requires working with real models in code to “design something that’s plausible and possible.”
> 
> Encounter reality as early as possible in the design process. Brian’s philosophy is to move designs from “napkin sketches” toward production code as quickly as possible. When you try designs in a browser instead of Figma, you immediately notice problems with loading states, screen sizes, and interactions that static designs hide.
> 
> The “prototype playground” is a shared Next.js app that centralizes all design prototypes. Instead of designers working in isolated repositories with different setups, this shared environment makes it easy to discover what others are working on and reuse code. The repository organizes prototypes by designer name and provides shared components for Notion-style UI elements.
> 
> Brian found it impossible to design good AI experiences in Figma: “You can design what the chat input looks like ... but what you can’t design in Figma is what it actually will feel like to use that thing.” Code prototypes connected to real AI models are essential for understanding edge cases and failure modes.
> 
> When Claude asks you to do something, teach it to do that thing itself. Brian’s most important rule for working with AI is to avoid manual intervention. For example, instead of manually checking if a prototype works in the browser, teach Claude to launch Chrome, test the functionality, and verify the results.
> 
> Claude Skills can solve specific recurring problems. When AI consistently hallucinated icon names (using “search” instead of “magnifying glass”), Brian created a skill that programmatically searches for icons and their synonyms across thousands of files. This demonstrates how AI can be taught to overcome its own limitations.
> 
> Custom slash commands dramatically simplify complex workflows. Brian created commands like “/figma” that handle everything from checking if MCPs are installed to extracting designs, implementing them as code, and verifying the results through multiple iterations. This makes advanced AI techniques accessible to less-technical team members.


https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-how-notions?utm_source=post-email-title&publication_id=10845&post_id=188306621&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true