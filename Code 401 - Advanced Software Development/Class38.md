# Class 38 Summary:

## Redux - Asynchronous Actions :

### How granular should your reducers be?

  * "There should be a separate reducer function for each slice of data. They are combined before being put into the store".

### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched.

  * "This is a Con because you may fire off reducers that you did not intend".

### Name a strategy for preventing the above
  
   * "You can use more specific names that represent the reducer and data want to change".


### Document the following Vocabulary Terms :  

| Term      |                                                   |
| -----------  | ----------------------------------------------------------------|
|store |holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it. |
|combined reducers |helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore. |

### Redux Fundamentals:
   * "use the React-Redux library to let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a Provider component to give those hooks access to the store".

### Redux Middleware and Side Effects:

  * "Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function". Some common kinds of side effects are things like:
     1. Logging a value to the console
     2. Saving a file
     3. Setting an async timer
     4. Making an AJAX HTTP request
     5. Modifying some state that exists outside of a function, or mutating arguments to a function
     6. Generating random numbers or unique random IDs (such as Math.random() or Date.now())

  * "Redux middleware were designed to enable writing logic that has side effects".

### Using Middleware to Enable Async Logic :

  * "We could have our middleware check to see if the "action" is actually a function instead, and if it's a function, call the function right away. That would let us write async logic in separate functions, outside of the middleware definition".

![image1](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

### Using the Redux Thunk Middleware :

  * "The thunk middleware allows us to write functions that get dispatch and getState as arguments. The thunk functions can have any async logic we want inside, and that logic can dispatch actions and read the store state as needed".

### Understanding Asynchronous Redux Actions with Redux Thunk :

  * "There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga".

  * "Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation".

  * "Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed".


#### Sources:
[source1](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

[source2](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)

