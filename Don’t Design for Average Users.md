---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> Engagement follows power laws, Zipf distributions, and log-normal skews
> 
> Stop designing for these ghosts and start designing for the radical asymmetry between the median (P50) and the 95th percentile (P95) user
> 
> The P95 user is not just a frequent visitor; they are the economic engine that subsidizes the P50 user’s experience
> 
> A mature product should therefore track at least four separate tails: usage volume, revenue, support cost, and strategic value
> 
> Why p95/p50 varies
> 	1. Task structure
> 	2. Role heterogeneity - %ile analysis should be paired with job to be done analysis, other you will design for a generic "power user" instead of specific personas
> 	3. Friction and infra - when usage is not punished by capacity, inconvenience or pricing, then heaviest users will pull farther away
> 	4. Metric choice - different metrics point to different problems
> 	5. Compounding returns - when more use produces more value, the upper tail becomes self-reinforcing
> 	6. Organizational maturity - supporting systems - templates, norms, training, etc
> 
> p95/p50 increasing often means tail expansion - product change that amplifies power users, or bad analytics
> p95/p50 decreasing can mean tail compression - rate limiting, outages affecting heavy users, or logging change
> Cohort the ratio by user age - new, activated, retained, and veteran
> 
> P50 tourist - Fragile, transactional and friction-averse
> 	Highly friction-averse - I have experienced this in some products which want to make me a power user right away
> 	Objective - activation and retention
> 	Conceal complexity and lower cognitive load
> 
> P95 whale - Unbounded, demanding and the engine of value
> 	5% of users who drive 80% of revenue, content and network effects
> 	Objective - service quality, customization
> 	Service quality must be judged by 95-99%ile of requests - already know this
> 	When a whale complains about missing an advanced feature, don't dismiss it as an edge case
> 		Power users are early indicators of where the market is going - they hit edge cases, invent workarounds and reveal which advanced features are quietly becoming core workflows
> 	Design defenses against the negative whale - tiny fraction of extreme users can generate the vast majority of server costs, support tickets, etc
> 
> Design a layered interface featuring progressive disclosure
> 	1. Build the simple on-ramp - Surface must be optimized for the p50 tourist
> 		Focus on 20% of the features that drive 80% of standard usage
> 		Assume 0 attention span and desire to learn
> 		Hide settings, advanced configs
> 		Make primary CTA obvious
> 	2. Excavate deep, uncapped wells of values - Progressively reveal advanced capabilities
> 		Do not ask novices to self-identify as advanced
> 		Reveal power features when behavior shows readiness - repeated use, larger batch sizes, shortcut adoption, recurring tasks, or attempts to export and automate
> 		The cleanest expert experience is often the one that stays out of sight until the moment it becomes useful
> 		Allow whales to build on top of your product
> 	3. Decouple time from monetization - Design UX loops that allow for infinite investment
> 		Do not put artificial friction in front of a whale who is trying to give you money or generate highly engaging content
> 		Design goal - unbounded utility, not endless activity
> 	4. Bridge the gap - Build pathways that pull the most motivated p50 users up the curve toward p95 status
> 		UX gamification, algo recs, habit forming design loops come into play here
> 		Track what % of p50->p75, p75->p95, etc
> 		Gen AI can help here with intention translation - prompt augmentation, agents can execute complex workflows
> 	5. Reconcile the buyer vs the user
> 		In b2b enterprise software, the buyer is frequently a p50 tourist who rarely logs in, except to check high level ROI dashboards
> 		While your product must deliver unbounded complexity for the whale who uses it daily, your reporting and administrative interfaces must be radically frictionless to satisfy the tourist who actually pays for it
> 		If your interfaces caters exclusively to the whale's complex workflows, it may overwhelm the executive during a sales demo and cost you the contract
> 
> Pricing strategy
> 	If p95/p50 is low, flat pricing is often best
> 	If p95/p50 is high, charge extra for heavy use
> 
> Churn analysis
> 	Weight user segments by their usage ratios - losing a whale costs far more than losing a median user
> 	Prioritize high volume users with dedicated support, advanced feature roadmaps, and community recognition
> 
> For product decisions, track the distribution

https://jakobnielsenphd.substack.com/p/p50-vs-p95?utm_source=tldrdesign