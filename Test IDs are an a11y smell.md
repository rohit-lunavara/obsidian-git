---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> The more your tests resemble the way your software is used, the more confidence they can give you.
> 
> If we focus our tests on what the user can see and interact with, we get the best bang for our buck: We’re free to refactor internals, layout things differently or change how API calls are made without having to change our tests
> 
> ```screen.getByRole('button', { name: 'Open Widget' }).click()```
> 
> If we’re using role-based selectors in our tests, we get a couple of things almost for free:
> 	1. We're doing some a11y testing
> 	2. Our tests become more readable
> 
> If those selectors don’t work, I know I have to change my app because it’s not accessible enough
> 	1. Use semantic HTML - it has implicit ARIA roles
> 	2. Ensure interactive elements have an accessible name - visible text or a proper label
> 	3. Use the keyboard to navigate around your app and look for something you can't use
> 	4. Use headings, landmarks and grouped regions to give the UI a clear structure
> 	5. Always associate form controls with labels so they can be found by name - can hide label
> 	6. Use browser devtools to switch between DOM tree and Accessibility tree view when inspecting elements
> 	7. Ask AI agents about a11y
> 
> If your tests can’t find it with a role-based selector, some of your users probably can’t either 
> In those cases, it’s better to fix the UI rather than work around it in the test by adding a `data-testid`

https://tkdodo.eu/blog/test-ids-are-an-a11y-smell