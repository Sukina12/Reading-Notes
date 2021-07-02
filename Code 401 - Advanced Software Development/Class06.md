# Class 06 Summary :

### Explain what a “Singleton” is (in Computer Science terms) ?

* A singleton  : "is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself".

### Explain how the Singleton pattern can be used with Node modules, specifically with classes :

* "The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times".

* "After we instantiate once, every time we call to instantiate again, it will not create another instance.. instead it will refer to only one instantiation (the first one)".

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it? 

* "The app.get() function is Application-level Middleware. the parameters passed to the method are req, res, and next. These are the incoming request, the response being written, and a method to call to pass the call to the next middleware function once the current middleware is finished. In this case, once the response is sent, the function exits. You could also chain other middleware here by calling the next() method.

### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| Router Middleware   | what it does actualy is to take the original request, and forward it to a sub handler according to the path |
| Dynamic Module Loading |function-like form of import that returns a promise of the requested module  |
| Singleton Pattern    |is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.    |
| CRUD -> REST Method Matches   | Create --> POST , Read --> GET , Update --> PUT , Delete --> DELETE |
| Mock Testing    |is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. |


### Securing Passwords with Bcrypt Hashing Function :

* "Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have".

### Basic access authentication :

* "basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :".

### OWASP auth cheatsheet :

* "Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know".

* "Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction". 

### Sources :

[source1](https://www.techopedia.com/definition/15830/singleton)
[source2](https://developer.okta.com/blog/2018/09/13/build-and-understand-express-middleware-through-examples)
[source3](https://refactoring.guru/design-patterns/singleton)
[source4](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
[source5](https://en.wikipedia.org/wiki/Basic_access_authentication)

