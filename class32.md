How granular should your reducers be?

I would say that the default solution would be that a change of any of those attributes would trigger a separate kind of action such as CHANGE_EMAIL or CHANGE_NAME. And sometimes such granularity is good and valuable because different reducers, different parts of your application might need to react differently to those actions. Sometimes it might be much easier for reducers if they can distinguish between those two particular use-cases.


Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
Pro

Name a strategy for preventing the above

Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished

Document the following Vocabulary Terms
Term
store

A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it. A store is not a class. It's just an object with a few methods on it. To create it, pass your root reducing function to createStore .


combined reducers

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. ... First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers.


