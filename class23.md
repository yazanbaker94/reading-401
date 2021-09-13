Why do we not need more .html pages in a multi-page React app?
Because react allows us to use HTML in the render functions and rendered it all at the virual DOM in the index.html


If we wanted a component to show up on every page, where would we put it and why?



Inside the <BrowserRouter />, outside a <Route />
We would do that so it's not in a specific Route and always in all the Routes which is grouped by the browserRouter component.

What does routing do with the components that were rendered when a new route is requested
It will remove them and display the new ones.

What does props.children contain?
 a special prop that is passed to components automatically. The component has all the children properties that are inside the props.
 
How do useState() and this.setState() differ?

setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.



Term
State Hook

A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later.



Mounting and Un-Mounting

The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by "mounting" (adding nodes to the DOM), "unmounting" (removing them from the DOM), and "updating" (making changes to nodes already in the DOM).

