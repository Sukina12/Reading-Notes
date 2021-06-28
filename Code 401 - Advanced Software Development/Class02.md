# Class 02 Summary :

### What’s the difference between PUT and PATCH ?

* "PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely".

* "PATCH applies a partial update to the resource, Submits a partial modification to a resource. If you only need to update one field for the resource, you may want to use the PATCH method.".

### 3 services or tools that allow you to “mock” an API for development :

1. MockServer
2. Mockoon 
3. Postman Mock Server
4. Wiremock

### Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call? 

* "APIDoc transforms comments from inline documentation into API documentation. When you edit routes, it is straightforward to update documentation side by side with the code. APIDoc can also be used to create a list of places to look for the comments in the source code".

* Informational responses (100–199)
* Successful responses (200–299)
* Redirects (300–399)
* Client errors (400–499)
* Server errors (500–599)

### Compare and contrast SOAP and ReST :

* SOAP stands for Simple Object Access Protocol, REST stands for Representational State Transfer.

* SOAP is a protocol. SOAP was designed with a specification. It includes a WSDL file which has the required information on what the web service does in addition to the location of the web service.

* REST is an Architectural style in which a web service can only be treated as a RESTful service if it follows the constraints of being
  1. Client Server
  2. Stateless
  3. Cacheable
  4. Layered System
  5. Uniform Interface 

* SOAP uses service interfaces to expose its functionality to client applications, REST use Uniform Service locators to access to the components on the hardware device. 

###  Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| Web Server    |  computer software and underlying hardware that accepts requests via HTTP, the network protocol created to distribute web pages, or its secure variant HTTPS.                             |
| Express     |  a back end web application framework for Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs. It has been called the de facto standard server framework for Node.js                                                        |
| Routing      |   refers to how an application’s endpoints (URIs) respond to client requests.                                                       |
| WRRC      |    web request/response cycle traces how a user’s request flows through the app. 

### Preparation Materials :

##### An introduction to NodeJS and Express :

* Node : is an open-source environment that allows developers to create server-side tools and applications in javascript.
* We can use Node.js to create a simple web server using the Node HTTP package.                                               |

* Express : is the most popular node web framework, and is the underlying library for a number of other popular node web frameworks.

##### What is NPM? 

* npm is an open source software registry. the developers use it to show and borrow packages.

* npm consists of three distinct components :
  1. website
  2. command line interface 
  3. registry

* NPM using for :
  1. download standalone tools.
  2. share code with any npm user, anywhere.
  3. create organizations to coordinate package maintences and coding.
  4. find other developers who are working on similar problems and projects.

##### What is TDD? 

* "Test-driven development refers to a style of programming in  three activities: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)".

* Test-Driven Development starts with designing and developing tests for every small functionality of an application. TDD framework instructs developers to write new code only if an automated test has failed. This avoids duplication of code. The TDD full form is Test-driven development.

##### CI/CD :

* "Continuous integration (CI) and continuous delivery (CD) embody a culture, set of operating principles, and collection of practices that enable application development teams to deliver code changes more frequently and reliably."

* "Continuous integration is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently."

* "CD automates the delivery of applications to selected infrastructure environments. Most teams work with multiple environments other than the production, such as development and testing environments, and CD ensures there is an automated way to push code changes to them."

## Sources : 
[source1](https://rapidapi.com/blog/put-vs-patch/)
[source2](https://www.guru99.com/comparison-between-web-services.html)
[source3](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
[source4](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))
[source5](https://www.infoworld.com/article/3271126/what-is-cicd-continuous-integration-and-continuous-delivery-explained.html)