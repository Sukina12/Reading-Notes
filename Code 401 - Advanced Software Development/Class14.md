# Class 14 Summary :

### What’s the difference between a FIFO and a standard queue?
  * "Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it".

### How can the server be assured a message was properly received?
  * "Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer".

### What classic design pattern is best represented by event driven programming?
  * Event-driven from end to end.

### How do you test an event driven system?
  * "tests for event-driven systems operate on events for inputs and events for outputs. Another by-product of a decoupled architecture is often an absence of mocks and stubs in the service test code, which stems from inherent ‘unawareness’ the service has of other services".

### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|FIFO Queue | FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated. |
|Pub/Sub | enables you to create systems of event producers and consumers, called publishers and subscribers.  |

### AWS SNS and SQS :

  * SNS : " is a web service that makes it easy to set up, operate, and send notifications from the cloud. It provides developers with a highly scalable, flexible, and cost-effective capability to publish messages from an application and immediately deliver them to subscribers or other applications".

  * SNS benefits:
    1. nstantaneous, push-based delivery (no polling)
    2. Simple APIs and easy integration with applications
    3. Flexible message delivery over multiple transport protocols
    4. Inexpensive, pay-as-you-go model with no up-front costs 

  * SQS : "is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components" .

  ![image1](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2017/11/20/introducing_sns_message_filtering_image_4.png)

### Sources:
[source1](https://aws.amazon.com/sqs/faqs/)
[source2](https://aws.amazon.com/message-queue/)
[source3](https://medium.com/dan-on-coding/testing-event-driven-systems-63c6b0c57517)
[source4](https://aws.amazon.com/sns/faqs/)

