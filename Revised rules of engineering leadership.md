---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> # Revised Rules of Engineering Leadership — Will Larson
> 
> ## Core idea
> 
> AI has dramatically increased execution speed in engineering.
> 
> The main constraints are no longer:
> - writing first-pass code
> - performing migrations
> - manual repetitive workflows
> 
> The bottlenecks are increasingly:
> - judgment
> - development harness quality
> - organizational alignment
> - decision-making speed
> 
> ---
> 
> # Revised Rules
> 
> ## 1. Migrations can often be done by individuals, not teams
> 
> Large technical migrations that previously required many engineers can now often be driven by one engineer or a very small team.
> 
> AI reduces migration effort to ~10% of prior cost.
> 
> ### Implications
> - Individual leverage is much higher
> - Individual judgment matters more
> - Small mistakes now have larger downstream impact
> 
> Important:
> Migration speed increased, but migration quality matters more.
> 
> ---
> 
> ## 2. First-pass code is cheap; working code is not
> 
> Generating code is easy.
> 
> Reliable production code still depends on engineering infrastructure.
> 
> ### Development harness includes
> - tests
> - CI/CD
> - validation environments
> - preview environments
> - safety checks
> 
> Core insight:
> AI lowers code generation cost, not correctness cost.
> 
> Bad harness → fast production of bugs.
> 
> ---
> 
> ## 3. Optimize processes for agents
> 
> Most routine process steps can be automated.
> 
> Examples:
> - issue triage
> - code review
> - repetitive investigations
> - workflow execution
> 
> ### Principle
> Design processes assuming agents handle the common case.
> 
> Humans focus on:
> - edge cases
> - high-risk changes
> - judgment-heavy work
> 
> ---
> 
> ## 4. Traditional sprint planning is too low-level
> 
> Weekly or biweekly task planning becomes less useful when execution accelerates.
> 
> Humans should plan at higher abstraction levels.
> 
> Focus on:
> - priorities
> - strategy
> - constraints
> - decision boundaries
> 
> Not micro-task scheduling.
> 
> ---
> 
> ## 5. Durable, high-ownership teams matter more
> 
> AI improves execution but does not replace domain understanding.
> 
> Persistent teams accumulate:
> - context
> - ownership
> - intuition
> - system knowledge
> 
> These enable better decisions.
> 
> ### Key insight
> Doing things faster matters less than doing the right thing.
> 
> Domain context remains critical.
> 
> ---
> 
> ## 6. AI-first companies will not just be tiny genius teams
> 
> There is a popular idea:
> small elite engineering teams will build everything.
> 
> Larson disagrees.
> 
> Why:
> Even highly capable individuals hit limits without domain context.
> 
> Sustainable execution still depends on teams.
> 
> ### Conclusion
> Durable teams remain the core organizational unit.
> 
> ---
> 
> ## 7. Fast, good, durable decision-making is now essential
> 
> AI only creates value if organizations can act on faster execution.
> 
> Examples:
> - legal automation requires legal approval
> - feature implementation requires launch decisions
> - architectural change requires commitment
> 
> Main constraint becomes decision latency.
> 
> ---
> 
> ## CTO role is becoming more technical
> 
> Because faster execution creates more decisions, leadership must resolve disagreements quickly.
> 
> CTOs increasingly need:
> - technical depth
> - architectural judgment
> - ability to make binding decisions
> 
> Less bureaucracy, more technical leadership.
> 
> ---
> 
> # Practical Examples from Imprint
> 
> ## Deployment migration
> - Went from ~6 deploys/week to 200–400 deploys/week
> - Engineering headcount doubled
> - Deployment frequency improved 20–30x
> - Migration mostly done by two infra engineers
> 
> ---
> 
> ## AI adoption
> - January: ~25% used AI coding tools daily
> - February: 100% adoption
> - No mandate required
> - Adoption happened by reducing friction
> 
> Result:
> Most PRs now begin with AI-generated first drafts.
> 
> ---
> 
> ## Configuration migration
> Many configuration systems unified into only two systems.
> 
> Previously a multi-year effort.
> 
> Completed in less than one quarter using small focused efforts.
> 
> ---
> 
> ## Frontend monorepo migration
> Multi-repo frontend moved to monorepo.
> 
> - Done mostly by one engineer
> - Completed in ~1 month
> 
> Benefits:
> - shared tooling
> - cheaper library maintenance
> - reduced package friction
> 
> ---
> 
> ## Static typing migration
> Frontend code moved from mostly untyped to fully typed.
> 
> Done by one engineer over a few weeks.
> 
> ---
> 
> ## npm → pnpm migration
> Completed by one engineer in a few days.
> 
> Benefits:
> - better security defaults
> - faster deploys
> 
> ---
> 
> # Lessons on harness quality
> 
> Low-quality AI output is harmful.
> 
> Examples:
> - sloppy PRs
> - weak design docs
> - poor context
> 
> These create cleanup cost and degrade future AI performance.
> 
> Good AI usage requires:
> - ownership
> - validation
> - post-deployment monitoring
> 
> ---
> 
> # Agent-first workflow examples
> 
> ## Issue triage automation
> Customer operations issues are triaged by an AI harness.
> 
> Harness uses:
> - team knowledge
> - open tickets
> - warehouse data
> 
> Humans handle exceptions.
> 
> ---
> 
> ## Automated code review
> AI performs first-pass review.
> 
> Humans provide higher-value feedback.
> 
> ---
> 
> ## Cross-company automation
> Other teams automate workflows too.
> 
> Example:
> Fraud team automates initial attack investigation.
> 
> ---
> 
> ## Tooling shift
> Moved:
> - from Jira
> - to Linear
> 
> Reasons:
> - better MCP support
> - better Slack integration
> - better agent workflows
> 
> ---
> 
> # Organizational lessons
> 
> Main blockers to AI leverage are still old problems:
> 
> - organizational misalignment
> - unclear decisions
> - poor architecture
> 
> AI increased execution speed.
> 
> It did **not** remove the need for:
> - good structure
> - good leadership
> - good judgment
> 
> ---
> 
> # Final takeaway
> 
> AI changes the economics of execution.
> 
> The scarcest resources are now:
> 
> 1. Judgment  
> 2. Technical architecture  
> 3. Organizational alignment  
> 4. Fast, durable decision-making

https://lethain.com/revised-rules-of-engineering-leadership/?utm_source=lethain&utm_medium=email&utm_campaign=revised-rules-of-engineering-leadership-198a