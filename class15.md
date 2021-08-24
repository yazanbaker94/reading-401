What’s the difference between a FIFO and a standard queue?

Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.


How can the server be assured a message was properly received?
the client sends a message that he received it and emits a message back that it's all good and the server can delete it now.


What classic design pattern is best represented by event driven programming?

An Event-Driven Architecture for data and applications is a modern design approach centered around data that describes “events” (i.e., something that just happened). Examples of events include the taking of a measurement, the pressing of a button, or the swiping of a credit card.

How do you test an event driven system?

Unit Tests
Unit tests are the most basic tests you will write. The SUT in this case is typically an individual class. Let’s say, the Payment Service needs to apply a sales tax, based on the customer’s location

service Tests
Service tests, as the name suggests, treat the entire service as the SUT, and increasingly, in microservice architectures this is where the bulk of automated testing occurs. These tests verify the contract of services, that is — given certain inputs, the service produces a certain output. 

End-to-end Tests
The final level of tests we will discuss here is the end-to-end tests. This is the ultimate ‘it works’ validation, that ensures that the contracts covered in the service tests ‘meet’. 


FIFO Queue

For a FIFO (First in First out Queue), the element that goes first will be the first to come out. For a LIFO (Last in First out Queue), the element that is entered last will be the first to come out. An item in a queue is added using the put(item) method. To remove an item, get() method is used.


Pub/Sub
Pub/Sub allows services to communicate asynchronously, with latencies on the order of 100 milliseconds.

Pub/Sub is used for streaming analytics and data integration pipelines to ingest and distribute data. It is equally effective as messaging-oriented middleware for service integration or as a queue to parallelize tasks.



