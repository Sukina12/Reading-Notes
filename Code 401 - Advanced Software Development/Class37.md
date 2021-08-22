# Class 37 Summary:

##  Redux - Combined Reducers :

### Why choose Redux instead of the Context API for global state?

  * "Redux is much more powerful and provides a large number of features that the Context Api doesn't provide, Also, React Redux uses context internally but it doesn’t expose this fact in the public API. So you should feel much safer using context via React Redux than directly because if it changes, the burden of updating the code will be on React Redux instead developer responsibility".

### What is the purpose of a reducer?

  * "takes the previous state and an action, and returns the next state".

### What does an action contain?

  * "a type property and any other data that it needs to describe the action".

### Why do we need to copy the state in a reducer?

  * " if we change values inside an object and we want to know if something has changed, we'd have to make a full copy so we can store individual properties, and then compare each property of the new and old object to determine what, if anything, has changed".

### Document the following Vocabulary Terms :  

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|immutable state | is state that cannot be changed.  |
|time travel in redux | the ability to move back and forth among the previous states of an application and view the results in real time  |
|action creator |is merely a function that returns an action object  |
|reducer | a function that receives the current state and an action object, decides how to update the state if necessary, and returns the new state |
|dispatch |The only way to update the state is to call store.dispatch() and pass in an action object.  |

### Using combineReducers :

#### Core Concepts : 
  * "The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object".

#### There are several important ideas to be aware of when using combineReducers :

  1. "First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario".

  2. While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors.

  3. "One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, combineReducers has specific behavior that does work that way".

  4. "You can use it at all levels of your reducer structure, not just to create the root reducer. It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer".

#### Defining State Shape :
  * There are two ways to define the initial shape and contents of your store's state:
     1. "The createStore function can take preloadedState as its second argument".
     2. " for the root reducer to return the initial state value when the state argument is undefined".

##### combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys.

##### The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

##### Any reducer passed to combineReducers must satisfy these rules: 
  1. "For any action that is not recognized, it must return the state given to it as the first argument".

  2. "It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else".

  3. "If the state given to it is undefined, it must return the initial state for this specific reducer". 

##### ou may call combineReducers at any level of the reducer hierarchy. It doesn't have to happen at the top. In fact you may use it again to split the child reducers that get too complicated into independent grandchildren, and so on.


#### Sources :
[source1](https://www.fullstack.cafe/blog/top-26-react-redux-interview-questions-to-brush-up-2018)
[source2](https://www.pluralsight.com/guides/how-to-write-redux-reducer)
[source3](https://read.reduxbook.com/markdown/part1/03-updating-state.html)
[source4](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)



