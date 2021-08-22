What is the benefit of transforming data into packets?


Packets are the basic units of communication over a TCP/IP network. Devices on a TCP/IP network divide data into small pieces, allowing the network to accommodate various bandwidths, to allow for multiple routes to a destination, and to retransmit the pieces of data which are interrupted or lost.


UDP is often refereed to as a connectionless protocol. Why is this?

UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt. Examples of applications that use connectionless transport services are broadcasting and tftp


Can a socket server application have multiple socket connections?

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to


Can a socket connection application be connected to multiple socket servers?

A connected socket is assigned to a new (dedicated) port, so it means that the number of concurrent connections is limited by the number of ports, unless multiple sockets can share the same port

Can an application be both a socket server and a socket connection?

However, if you want to use a client socket and a server socket within a single application, then yes! You can do that if you're willing to use two different ports. Or if the sockets won't be using the same port at the same time.




Observer Pattern
The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods



Listener

An event listener is a procedure or function in a computer program that waits for an event to occur. ... The listener is programmed to react to an input or signal by calling the event's handler. The term event listener is often specific to Java and JavaScript



Event Handler

An event handler is a callback routine that operates asynchronously and handles inputs received into a program (events). ... Nearly all software architectures must include at least some event handling capabilities, if only to deal with out-of-bounds conditions and errors.


Event Driven Programming

In computer programming, event-driven programming is a programming paradigm in which the flow of the program is determined by events such as user actions 

Event Loop

n computer science, the event loop is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider", then calls the relevant event handler.

Event Queue

An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

Call Stack

In computer science, a call stack is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, program stack, control stack, run-time stack, or machine stack, and is often shortened to just "the stack"

Emit/Raise/Trigger

In node. js an event can be described simply as a string with a corresponding callback. An event can be "emitted" (or in other words, the corresponding callback be called) multiple times or you can choose to only listen for the first time it is emitted


The trigger() method triggers the specified event and the default behavior of an event (like form submission) for the selected elements. This method is similar to the triggerHandler() method, except that triggerHandler() does not trigger the default behavior of the event.



Subscribe

The subscriber function defines how to obtain or generate values or messages to be published. To execute the observable you have created and begin receiving notifications, you call its subscribe() method, passing an observer. This is a JavaScript object that defines the handlers for the notifications you receive.

database

a structured set of data held in a computer, especially one that is accessible in various ways.
"a database covering nine million workers"

