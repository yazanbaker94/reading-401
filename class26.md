Describe use cases useState() vs useReducer()

Should I use Usestate or Usereducer?
useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

Why do custom hooks need the use prefix?

Custom Hooks
This is mainly to have an extra option for sharing state and logic between components. ... Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.


What do custom hooks usually do?

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.


Using any list of custom hooks, research and name one that you think will be useful in your applications

useClippy
A hook for copying data to the clipboard and retrieving/pasting it using Ctrl-C/Command-C and Ctrl-V/Command-V.

useBrowserContextCommunication
useBrowserContextCommunication uses the Broadcast Channel API to deliver an easy solution for communication between different browser contexts (tabs, iframes, windows).


useScript
useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

useLocalStorage
This hook simplifies the storage and retrieval of data from the localStorage.


useIdb
UseIdb uses the IndexedDB storage in the browser to store data. IndexedDB is not as popular or as known as its counterpart localStorage but it definitely shouldn’t be overlooked.



6. use-mouse-action

A library with three React hooks for listening to mouse events on an element or JSX element.


useOnlineStatus
useOnlineStatus uses the navigator.onLine property to check the network status to determine if the user is connected to the internet or not.


useDocumentTitle
As you probably know, routing in React apps doesn’t automatically update the page title (shown in the browser’s tabs). useDocumentTitle hook helps to solve exactly that.




Describe how a hook that fetches API data might work

Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = "https://api.adviceslip.com/advice"; const fetchData = async () => { try { const response = await fetch(url); const json = await response. json(); console. log(json); } catch (error) { console.



Term
reducer

Definitions of reducer. a substance capable of bringing about the reduction of another substance as it itself is oxidized; used in photography to lessen the density of a negative or print by oxidizing some of the loose silver. synonyms: reducing agent, reductant. types: hydrazine.
