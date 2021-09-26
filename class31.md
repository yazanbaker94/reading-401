Why choose Redux instead of the Context API for global state?

Redux helps you manage "global" state - state that is needed across many parts of your application. The patterns and tools provided by Redux make it easier to understand when, where, why, and how the state in your application is being updated, and how your application logic will behave when those changes occur.Jan


What is the purpose of a reducer?

A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently


What does an action contain?

An action is an object that contains two keys and their values. The state update that happens in the reducer is always dependent on the value of action


Why do we need to copy the state in a reducer?

If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.





Document the following Vocabulary Terms
Term
immutable state
In object-oriented and functional programming, an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created.


time travel in redux

The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. ... This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

action creator

An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.


reducer

Reducers are functions that take the current state and an action as arguments, and return a new state result. In other words, (state, action) => newState .


dispatch

dispatch() is the method used to dispatch actions and trigger state changes to the store. react-redux is simply trying to give you convenient access to it. Note, however, that dispatch is not available on props if you do pass in actions to your connect function

