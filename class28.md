Why is the Context API useful?

The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application


Can a component outside of a provider get its context?

With the introduction of react-hooks in v16.8.0, you can use context in functional components by making use of useContext hook


What are some common use cases for using the Context API?

Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.


Describe “Context Hell”

Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.

Document the following Vocabulary Terms
Term


global state
Global states are used when components need to share states. React provides a very good and simple way to manage local state(React hooks) but when it comes to global state management the options available are overwhelming.

global context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

provider
The <Provider> component makes the Redux store available to any nested components that need to access the Redux store. Since any React component in a React Redux app can be connected to the store, most applications will render a <Provider> at the top level, with the entire app's component tree inside of it.
  
consumer
  
  Context.Consumer
A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.
  
  
  
