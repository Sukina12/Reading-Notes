# Class 19 Summary :

## AWS: Events 

### Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server :

  * "Amazon’s API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. With a few clicks you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any Web application. Amazon API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management".

  * "Express Gateway is an API Gateway that can sit at the heart of any microservices architecture, regardless of what language or platform you’re using. Express Gateway secures your microservices and exposes them through APIs using Node.js, ExpressJS and Express middleware".

### List the AWS Database offerings and talk about the pros and cons of each

![DataBase](https://user-images.githubusercontent.com/79833733/127128447-da637f46-67fc-4bae-a5b3-1b87711769cf.png)

### What’s the difference between a FIFO and a standard queue? 

  * "Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it".

### How can the server be assured a message was properly received?

  * "TCP ensures that packets have been delivered to connection peer, and will retransmit until they are, that only handles failures at the network layer. Acknowledgements and confirms indicate that messages have been received and acted upon by the peer application. An acknowledgement signals both the receipt of a message, and a transfer of ownership where the receiver assumes full responsibility for it".

###  Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|Serverless API  | is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.  |
| Triggers  | external events or circumstances that may produce very uncomfortable emotional or psychiatric symptoms, such as anxiety, panic, discouragement, despair, or negative self-talk.    |
|Dynamo vs Mongo  | DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas. ... DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents  | 
|Dynamoose vs Mongoose  | Dynamoose is a modeling tool for Amazon's DynamoDB,Mongoose is a modeling tool for Amazon's MongoDB | 

### AWS — Difference between SQS and SNS :

  * "SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS".

  * "SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll or pull messages from SQS. Messages can't be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later. Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers. SNS supports several end points such as email, SMS, HTTP end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS".

![image2](https://res.cloudinary.com/practicaldev/image/fetch/s--_rz9_IWG--/c_imagga_scale,f_auto,fl_progressive,h_720,q_auto,w_1280/https://dw71fyauz7yz9.cloudfront.net/video-upload__c8bc44f83cd41222de8ae55b55c63ef2/thumbs-video-upload__c8bc44f83cd41222de8ae55b55c63ef2-00001.png)

![image3](https://www.jeremydaly.com/wp-content/uploads/2019/01/sns-sqs-app.png)


#### Sources :

[source1](https://www.express-gateway.io/eg-vs-amazon-aws-api-gateway/)
[source2](https://aws.amazon.com/sqs/faqs/)
[source3](https://www.rabbitmq.com/reliability.html)
[source4](https://stackoverflow.com/questions/13681213/what-is-the-difference-between-amazon-sns-and-amazon-sqs)
