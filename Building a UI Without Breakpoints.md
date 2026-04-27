---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> Breakpoints were a major improvement over fixed desktop layouts
> 	There is nothing inherently wrong with this style. 
> 	The challenge appears at scale, where dozens of components with repeated viewport branches quickly increase CSS size, complicate overrides, and increase coupling between unrelated parts
> 	
> When components live in different containers, viewport-based rules can produce mismatched behavior, force unnecessary exceptions, and make component reuse less predictable
> 
> Method 1: Intrinsic Layouts First
> 	Instead of saying, “at width X, force N columns,” define constraints and let the browser derive the layout continuously
> 	**The Ubiquitous Card Grid** - Instead of hardcoding column counts at breakpoints, we can use `auto-fit` and `minmax()` to create a grid that naturally fills available space while respecting a minimum card width
> 	**Two-Region Flexible Layout** - Instead of switching from single-column to multi-column at a breakpoint, as many of us do, we can define a flexible layout that simply adapts
> 	
> Method 2: Use Fluid Values
> 	Typography, spacing, radius, and component size can usually be continuous instead of stepped.
> 	You can use min() and max() for continuous values, but clamp() is especially useful here because it gives you both a safe minimum and a safe maximum, with a fluid middle range.
> 	To get these `clamp()` values, you can use one of the many [clamps calculators](https://clamp-calculator.netlify.app/) out there. The result is a single rule that produces the same effect as multiple media queries, but with smoother scaling and less CSS
> 	
> Method 3: Container Units for Local Responsiveness
> 	In component-based systems, we often don’t know where a component will render or how much space it will actually get. This is exactly where **container units** become useful, and now that support is widely available, we can use them with confidence
> 	Container units are ideal when you want values to scale based on the component’s real rendered size, not the screen width
> 	
> Method 4: Container Queries for Real Structural Changes
> 	The important shift is that we’re no longer asking “How wide is the screen?”, we are asking “How much space does this specific component have right now?”. That makes the behavior reusable and predictable across sidebars, modals, cards, and full-page layouts
> 
> Intrinsic layouts handle structure, fluid values handle scale, container units handle local sizing, and container queries handle real structural shifts
> 
> Reframing Media Queries: Capabilities and Preferences
> 	The shift is not about removing media queries. It is about using them for what they are best at, understanding the device and the user environment, instead of measuring screen pixels for layout.
> 	e.g. we can detect hover support and pointer accuracy, adapt to display-mode, reduce expensive effects when updates are slow, and show fallback content when scripting is unavailable.
> 	
> Migration Checklist
> 	Audit existing media queries. Separate scalar changes (size, spacing, typography) from structural changes (composition/layout).
> 	Replace scalar branches first. Move to clamp(), min(), and max() tokens.
> 	Shift layout to intrinsic primitives. Prefer auto-fit and minmax() over fixed column counts tied to viewport widths.
> 	Scope behavior to the component. Add container-type and introduce container units where helpful.
> 	Add container queries only where structure changes. Keep thresholds local to the component.
> 	Keep media queries for environment intent. Favor hover, pointer, prefers-reduced-motion, and update.
> 	Validate in real placements. Test the same component in sidebar, modal, and full-content contexts.

https://frontendmasters.com/blog/building-a-ui-without-breakpoints/