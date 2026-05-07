---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> ![[Pasted image 20260508003129.png]]
> 
> Agents need mostly the same things humans need to work efficiently: boundaries, constraints, and fast feedback loops
> 
> Code that changes together should live together
> 
> Everything widget related code goes into src/widgets/. That can be components, that can be hooks, types, utils, constants, whatever.
> 	It doesn’t matter what it is technically, the only thing that matters is what it does.
> 
> Verticals - code that is grouped by functionality rather than technical layers
> 
> But What About Shared Code?
> 	the solution is usually to make them their own vertical
> 
> A lot of the time, shared code that’s not domain specific can and should come from your Design System
> 	If you don’t have one, create a top-level directory called `/design-system` and just have it be its own vertical
> 	The scope of a Design System is pretty clear: Reusable assets, components and patterns to ensure consistency in your product
> 
> Moving that code together, into its own vertical, immediately increases cohesion, but doesn’t automatically reduce coupling
> 	To fix that, we need boundaries
> 
> Can achieve this with monorepos - Every vertical gets its own package(lib) in the repo, with its own deps and public interface defined in the `package.json` exports field
> 	pnpm workspaces are pretty good for this
> 	workspaces - apps + libs/packages
> 	Inside libs, write shared code which will be explicitly imported by the apps
> 
> The catch:
> 	1. Choosing the correct vertical for each piece of code is hard
> 	2. Having "private" code runs the risk of multiple teams re-implementing the same things from scratch

https://tkdodo.eu/blog/the-vertical-codebase