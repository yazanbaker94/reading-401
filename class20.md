Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

Basically AWS has an API gateway where you can define the route that you want the end point to be, such as /getData, and Lambda is what the server should do once someone reaches to that endpoint.
In expressJS Server, we can also see that the same thing happens, where we define our own route, and create a function whether it is in the same code block or made outside and then imported, and therefore when someone visits that endpoint, he'd able to see what the function does, such as retrieve data.


List the AWS Database offerings and talk about the pros and cons of each
## Amazon RDS-A

Easy to use 
Amazon RDS Automatic software patching 
Amazon RDS Recommendation Engine
Amazon RDS Performance
RDS Instance Scalability
Amazon RDS Read Replicas 
Amazon RDS Availability 
Amazon RDS Security

CONS:
Patching forces a downtime
No scale-out for write workloads
Downtime required for scaling operations
No automated performance tuning
Not a zero-administration database



## Amazon DynamoDB
PROS:
Consistent and fast performance
Able to handle large sized data sets at an ease
Fast processing of data
Highly scalable on demand
Easy to set up with business intelligence applications to perform analytics on the data generated


CONS:
Can only be deployed on AWS
No support for triggers and joins
Limited support for querying the databases


 
 

What’s the difference between a FIFO and a standard queue?

A standard queue tries to preserve the order of messages (best-effort), but there is a possibility of a message being delivered out of order. In a FIFO queue, messages are grouped into “Message groups” and all messages within a message group are sent and received in strict order.


How can the server be assured a message was properly received?
The client/child will listen to the emitted socket from the server and when that is complete, then the client will emit a socket "received" back to the server and therefore the server will know for sure its over and delete it from the server side.
