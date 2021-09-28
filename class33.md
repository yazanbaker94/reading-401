What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.


When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

applyMiddleware


Document the following Vocabulary Terms
Term
middleware

software that acts as a bridge between an operating system or database and applications, especially on a network.


thunk

Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.

