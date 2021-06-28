# Class 04 Summary :

### Name 3 advantages to Test Driven Development:

1. reduce the time required for project development.
2. save project costs in the long run.
3. code flexibility and easier maintenance.

### In what case would you need to use beforeEach() or afterEach() in a test suite? 

* If we have some work we need to do repeatedly for many tests, we can use beforeEach and afterEach.

### What is one downside of Test Driven Development ?

* "Continuous Tweaking. For data structures and black box algorithms unit tests would be perfect, but for algorithms that tend to be changed, tweaked or fine tuned, this can cause a big time investment that one might claim is not justified. So use it when you think it actually fits the system and don't force the design to fit to TDD".

### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

* "The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance".
* "A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child".

### Why REST?

* "REST stands for Representational State Transfer. It is an architectural style originally described by Roy Fielding".
*"REST is primarily run over HTTP and is commonly used in Web APIs. Applications based on the REST architecture conform to several guiding principles and constraints".

### Document the following Vocabulary Terms :


| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| functionak programming  |   programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values. |
| Object-oriented programming  |  a programming paradigm that relies on the concept of classes and objects. It is used to structure a software program into simple, reusable pieces of code blueprints (usually called classes), which are used to create individual instances of objects.   |
| class     |  a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.   |
| super   | keyword is used to access and call functions on an object's parent.   |
| this    | keyword refers to the object it belongs to.     |
| TDD    | a style of programming in  three activities: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)   |
| Jest    | is a delightful JavaScript Testing Framework with a focus on simplicity.  |
| CI    | is the practice of merging all developers' working copies to a shared mainline several times a day.  |
|  REST   |  software architectural style that was created to guide the design and development of the architecture for the World Wide Web.   |
|   Data Model  | is defined as an abstract model that organizes data description, data semantics, and consistency constraints of data. The data model emphasizes on what data is needed and how it should be organized instead of what operations will be performed on data.  |

### SQL & NoSQL :

![SQL&NoSQL](https://image.slidesharecdn.com/sqlnosql-160421082635/95/sql-nosql-13-638.jpg?cb=1461228355)

* "NoSQL databases are flexible, scalable, and highly adaptable to the data management demands of modern businesses". 

*  "SQL and NoSQL—or, relational databases and non-relational databases. The difference speaks to how they’re built, the type of information they store, and how they store it. Relational databases are structured, like phone books that store phone numbers and addresses. Non-relational databases are document-oriented and distributed, like file folders that hold everything from a person’s address and phone number to their Facebook likes and online shopping preferences".




### Sources:
[source1](https://www.codica.com/blog/test-driven-development-benefits/)
[source2](https://stackoverflow.com/questions/64333/disadvantages-of-test-driven-development)
[source3](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up)
[source4](https://www.serviceobjects.com/resources/articles-whitepapers/why-rest-popular)
[source5](https://www.upwork.com/resources/sql-vs-nosql-databases-whats-the-difference?utm_source=google&utm_campaign=SEM_GGL_INTL_NonBrand_Marketplace_DSA&utm_medium=cpc&utm_content=113089129402&utm_term=&campaignid=11384804789&matchtype=b&device=c&gclid=Cj0KCQjw5uWGBhCTARIsAL70sLLUm32P1Pw0eDr04kPiO67E_kmVfguG-Z24CqDZ8JrkI18yXM2Uj_gaAhVkEALw_wcB)
[source6](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
