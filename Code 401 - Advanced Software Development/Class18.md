# Class 18 Summary :

## AWS: API, Dynamo and Lambda :

### What are serverless functions?

  * "is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier".

### If you were to create a system that emulated Lambda functions, how would you do it?

  * "Open the Functions page on the Lambda console.
      1. Choose Create function.
      2. Under Basic information, do the following:
         * For Function name, enter my-function.
         * For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

      3. Choose Create function.
  * Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources".

### Describe how a CDN works :

  * " (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. ... Without a CDN, content origin servers must respond to every single end user request".

  ![image1](https://www.ariseserver.com/wp-content/uploads/2017/02/Content-Delivery-Network-CDN.jpg)

###  Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|Serverless Functions | is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies.   |
| Cloud Storage   | Object storage for companies of all sizes. Store any amount of data. Retrieve it as often as you’d like.   |
| CDN   | (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user.   |

### Amazon API Gateway :

  * "Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests".

  * "API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation".

  * "API Gateway integrates with many other AWS services like AWS Lambda, AWS SNS, AWS IAM, and Cognito Identity Pools. These integrations allow for fully managed authentication and authorization layers, as well as detailed metrics and tracing for API requests".

  * Many AWS services support integration with Amazon API Gateway, including:
    1. AWS Lambda: run Lambda functions to generate HTTP API responses.
    2. AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
    3. Amazon Cognito: provide authentication and authorization for your HTTP APIs.

### API Types :
   1. RESTful APIs
   2. WEBSOCKET APIs

   ![image2](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2018/06/13/api-backends.png)

### What is DynamoDB? 

  * "is a hosted NoSQL database offered by Amazon Web Services (AWS)".

  * It offers :
    1. reliable performance.
    2. a managed experience.
    3. a small, simple API.

  * Benefits:
    1. Performance at scale.
    2. No servers to manage.
    3. Enterprise ready.

### Dynamoose :
   
  * "Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar".

  * Key Features:
    1. Type Safety.
    2. High level API.
    3. Easy to use syntax.
    4. Ability to transform data before saving documents.
    5. callback & promise support.

![image3](https://images.ctfassets.net/1d31s1aajogl/5ZcoOX41SWWPDJJDzVpBfE/eb2ae1d1c6ebbbd3a2176bec219dbf47/dynamodb_lambda_s3_static-hosting_architecture.png)


#### Sources :
[source1](https://blog.hubspot.com/website/serverless-functions)
[source2](https://docs.aws.amazon.com/lambda/latest/dg/getting-started-create-function.html)
[source3](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp)
[source4](https://www.serverless.com/amazon-api-gateway)
[source5](https://aws.amazon.com/api-gateway/)
[source6](https://www.dynamodbguide.com/what-is-dynamo-db/)
[source7](https://aws.amazon.com/dynamodb/)




