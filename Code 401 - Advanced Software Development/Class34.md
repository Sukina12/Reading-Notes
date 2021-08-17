# Class 34 Summary:

##  API Integration :

### How do bearer tokens work?
  * "The Bearer Token is created for you by the Authentication server. When a user authenticates your application (client) the authentication server then goes and generates for you a Token".

  * "The Bearer Token is normally some kind of opaque value created by the authentication server. It isn’t random; it is created based upon the user giving you access and the client your application getting access".

  * " To get an access token you send the Authentication server this bearer token along with your client id. This way the server knows that the application using the bearer token is the same application that the bearer token was created for".

### Describe express middleware
  * "Middleware literally means anything you put in the middle of one layer of the software and another. Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it’s attached to".

### What is a JWT?
  * "JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed".  

### Document the following Vocabulary Terms :  

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|role based access control  | is an approach to restricting system access to authorized users. It is an approach to implement mandatory access control (MAC) or discretionary access control (DAC).  |
|http cookies  |is a small piece of data that a server sends to the user's web browser. The browser may store it and send it back with later requests to the same server.  |


#### Sources:
[source1](https://www.devopsschool.com/blog/what-is-bearer-token-and-how-it-works/)
[source2](https://developer.okta.com/blog/2018/09/13/build-and-understand-express-middleware-through-examples)
[source3](https://jwt.io/introduction)


