---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> The Firefox security bug spike wasn’t just about the model; it was the harness too. While everyone focused on Mythos, the real story is that Firefox built a custom harness that gives AI agents the right tools to find, verify, and fix bugs. Brian says this is simpler than it looks: “It’s actually a reasonably simple wrapper around it. You just need to give it access to the right tools for the job.”
> 
> Agents are relentless in a way humans can’t be. Agents will try 14, 15, 20 different approaches to trigger a bug without getting tired or losing focus. Brian found bugs that required the agent to try 14 times before succeeding. As Brian notes, “Cognitive energy declines over time in a way that agents don’t.”
> 
> The verification loop is what eliminates false positives. Firefox uses a two-stage verification process: first, the agent must trigger an actual crash in their fuzzing build (a crystal-clear signal), and second, a verifier subagent checks that the bug report makes sense and doesn’t involve test-only configurations. By the time a bug reaches human engineers, there are almost no false positives.
> 
> Agents get laser-focused on the specific task and miss the bigger picture. When the patching agent fixed a bug, it would often patch just the one vulnerable location. Human engineers would then look at the fix and say, “This is right, but we should also check three other similar places in the codebase.”
> 
> Prioritization is essential when you have millions of lines of code. Firefox built a simple LLM judge that scores each file on two dimensions: likelihood of a memory safety issue, and ease of access from a webpage. Brian says this is “very, very simple” and anyone can replicate it.
> 
> The harness can be built in an afternoon using vendor SDKs. Firefox started with Claude’s agent SDK, which is essentially a wrapper around Claude Code CLI that streams JSON and provides programmatic hooks. Brian’s advice: use the vendor-provided harnesses (Claude agent SDK, OpenAI agent SDK) rather than third-party frameworks, because the models are likely post-trained to work best with their own infrastructure.
> 
> You should run multiple models and harnesses for security work. Because attackers will use whatever model and technique finds bugs, defenders need to scan with multiple approaches. Different models and harnesses spike on different strengths and will identify different vulnerabilities.
> 
> This approach works for more than security—performance, tech debt, and UX are all viable targets. The same pattern applies: score and prioritize areas of your codebase, give the agent a constrained goal with verification criteria, and plug the results into your existing pipeline. Brian says they’re doing active work on performance optimization using the same harness structure.

https://www.lennysnewsletter.com/p/how-i-ai-how-to-write-ai-agent-loops?utm_source=post-email-title&publication_id=10845&post_id=202479892&utm_campaign=email-post-title&isFreemail=false&r=969sr&triedRedirect=true