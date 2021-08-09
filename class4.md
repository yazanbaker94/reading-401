Name 3 real world use cases where you’d want to change the request with custom middleware
1. You need to square a number coming from the request.
2. You need to add a name into the request.
3. You need to console.log something into the request.


True or false: The route handler is middleware?
false

In what ways can a middleware function end the process and send data to the browser?
next()

At what point in the request lifecycle can you “inject” middleware?
After the request has been received.

What can cause express to error with “Request headers sent twice, cannot start a second response”

That particular error message is pretty much always caused because of a timing error in the handling of an async response that causes you to attempt to send data on a response after the response has already been sent.

It usually happens when people treat an async response inside an express route as a synchronous response and they end up sending data twice.



<hr><hr><hr><hr>

1. Middleware:  Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to.

2. Request Object - . The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

3. Response Object - . The res object represents the HTTP response that an Express app sends when it gets an HTTP request.
4. Application Middleware - Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next function in the application's request-response cycle. ... Middleware functions can perform the following tasks: Execute any code. Make changes to the request and the response objects.
5.  Routing Middleware - Routing defines the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware
6.  Test Driven Development - Test-driven development is the act of first deciding what you want your program to do (the specifications), formulating a failing test, then writing the code to make that test pass. It is most often associated with automated testing
7.  Behavioral Testing- What is Behaviour Testing? Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.




