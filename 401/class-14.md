# Read 14  - Event Driven Architecture : 
## What’s the difference between a FIFO and a standard queue?
Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

## How can the server be assured a message was properly received?
by recieving a response, else will throw an error.

## What classic design pattern is best represented by event driven programming?
Event-driven architecture (EDA) is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events. An event can be defined as "a significant change in state". For example, when a consumer purchases a car, the car's state changes from "for sale" to "sold".

## How do you test an event driven system?
There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application.
**Unit Tests**
Unit tests are the most basic tests you will write. The SUT in this case is typically an individual class. Let’s say, the Payment Service needs to apply a sales tax, based on the customer’s location. You would likely have a TaxCalculator class with a calculate() method, that accepts an Order argument and returns a double value representing the tax that needs to be applied to the total. Your unit test will interact with this class directly, passing various Order values to it, and verifying the tax has been calculated properly. At the unit level, the differences between a point-to-point and an event-driven system are insignificant, so we will not go deeper into it.
![img](https://miro.medium.com/max/700/1*NdiTTk_s6-ignfVB0fBKLw.jpeg)
**Service Tests**
Service tests, as the name suggests, treat the entire service as the SUT, and increasingly, in microservice architectures this is where the bulk of automated testing occurs. These tests verify the contract of services, that is — given certain inputs, the service produces a certain output. These tests execute in-memory (not a deployed service), prior to deployments and are mostly ‘cheap’ to run. Here is also where we begin to see substantial differences in test implementation between point-to-point and event-driven systems. The reason for these differences is a radically different collaboration style between services and hence — different contracts, that these tests need to cover.
We’ll start with a point-to-point system. The Payment System’s contract describes the HTTP request and response with its only consumer — the Order Service.
![img](https://miro.medium.com/max/700/1*cF7xwAC1pIlpLly8FMXflg.jpeg)
**End-to-end Tests**
The final level of tests we will discuss here is the end-to-end tests. This is the ultimate ‘it works’ validation, that ensures that the contracts covered in the service tests ‘meet’. In other words — these tests connect the dots between individual services and ensure that what service A needs, is in fact what service B is delivering. These tests typically execute post-deployment, against a test environment. They take longer to run and provide less focus in case of a failure, so they should be treated as the last bastion of defense.
These tests operate from a standpoint resembling that of a real user. In these tests, individual services and the specifics of a messaging platform are abstracted, meaning that rarely, at this level, will be interacting with Kafka directly. Here is what the System Under Test looks like:
![img](https://miro.medium.com/max/700/1*wQCWYjKoLkn8SekOEStHmQ.jpeg)