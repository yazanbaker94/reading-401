Explain what a “Singleton” is (in Computer Science terms)
A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object


Explain how the Singleton pattern can be used with Node modules, specifically with classes


A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there's already an instance, the singleton will create a new one. Let's take a look at where creating multiple instances of one object might create problems within our application


If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().

Error-handling middleware always takes four arguments. You must provide four arguments to identify it as an error-handling middleware function. Even if you don’t need to use the next object, you must specify it to maintain the signature. Otherwise, the next object will be interpreted as regular middleware and will fail to handle errors.

Define error-handling middleware functions in the same way as other middleware functions, except with four arguments instead of three, specifically with the signature (err, req, res, next)):

Built-in middleware
Starting with version 4.x, Express no longer depends on Connect. The middleware functions that were previously included with Express are now in separate modules; see the list of middleware functions.

Third-party middleware
Use third-party middleware to add functionality to Express apps.


Router Middleware

The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware.


Dynamic Module Loading

Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. 


Singleton Pattern

A Singleton is an object which can only be instantiated one time. Repeated calls to its constructor return the same instance and in this way one can ensure that they don't accidentally create, say, two Users in a single User application


CRUD -> REST Method Matches

                  Create = PUT with a new URI
                           POST to a base URI returning a newly created URI
                  Read   = GET
                  Update = PUT with an existing URI
                  Delete = DELETE

Mock Testing

Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. ... Such a service can be replaced with a mock object.

