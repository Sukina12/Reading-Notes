# Class 01 Summary:

### Node Ecosystem, TDD, CI/CD :

##### TDD :

* TDD (Test-driven development) : "is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases". (wikipedia)

##### CI/CD :

* CI/CD : "is a method to frequently deliver apps to customers by introducing automation into the stages of app development. The main concepts attributed to CI/CD are continuous integration, continuous delivery, and continuous deployment. CI/CD is a solution to the problems integrating new code can cause for development and operations teams (AKA "integration hell")".(redhat.com)

**********************************************************************

### Describe what Array.map() does :

* iterate over the elements in array, transform its elements and include the result in new array.

* example:

![map](https://www.itboy.in/wp-content/uploads/2021/01/map.png)


### Describe what Array.reduce() does :

* cycles through each number in the array and reduce the array to a single value by excuting function on each value and the return value of the function is dtored in an accumulator.

* syntax : array.reduce( function(total, currentValue, currentIndex, arr), 
initialValue ).

* example : 

![reduce](https://res.cloudinary.com/practicaldev/image/fetch/s---CsNi0td--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://cl.ly/635e6f8acce6/Image%25202018-09-19%2520at%252011.21.07%2520AM.png)


### Superagent: 

* SuperAgent : "is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js".

### Promises :

* Promise : "is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future".

![example](https://miro.medium.com/max/1024/1*yAFctUA8useVWRbC-nWhBA.png)

##### Promise.prototype.then() :

* example :

![then](https://miro.medium.com/max/700/1*Xt_kSc5t1QH8oeF4GeIZew.jpeg)

##### async / await :

* example :

![async](https://miro.medium.com/max/700/1*ktmJ30vivdMsrAgHwtuynw.jpeg)

###  Callback functions : 

* A callback function is a function that gets passed as an argument into a parent function call.

* A callback can be used synchronously or asynchronously.

* There's a difference in the order in which things happen in the timeline, depending on whether the callback is used synchronously or asynchronously.

##### asynchronous callback :

* example :

![asynch](https://res.cloudinary.com/practicaldev/image/fetch/s--5e204O-Y--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/rjqf7w2vmlxxz5ez0dbz.png)

##### synchronous callback :

![synch](https://res.cloudinary.com/practicaldev/image/fetch/s--dqZaqp09--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/hyaxexxqnkl9ymxrjlh4.png)



