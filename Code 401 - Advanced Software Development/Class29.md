# Class 29 Summary :

## Advanced State with Reducers :

### How can we ensure that an effect hook runs only once?

  * If we pass an empty array [] , it just renders the component only once like componentDidMount .

### Can useState() update more than one state variable at the same time?

  * "we could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn’t merge objects with existing state, it replaces the object entirely".

### Is useState() synchronous?

  * "useState and setState both are asynchronous, They do not update the state immediately but have queues that are used to update the state object. This is done to improve the performance of the rendering of React components".

### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|State Hook |the State of a component is an object that holds some information that may change over the lifetime of the component.and  Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.  |
|Component Lifecycle | Each component in React has a lifecycle which you can monitor and manipulate during its three main phases: Mounting, Updating, and Unmounting |

### useReducer Hook :

  * "useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications".

  * "useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second".

  * "useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks".

  * "There are two different ways to initialize useReducer state. You may choose either one depending on the use case. The simplest way is to pass the initial state as a second argument, You can also create the initial state lazily. To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg)".

  * There are three main building blocks in Redux:
     1. A store — an immutable object that holds the applications state data
     2. A reducer — a function that returns some state data, triggered by an action type
     3. An action — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property.
 
### The reducer function
  
  * "The reduce() method in JavaScript executes a reducer function on each element of the array an and then returns a single value. The reduce() method accepts a reducer function, which itself can accept up to four arguments".

  * "The reducer function itself accepts two parameters and returns one value. The first parameter is the current state, and the second is the action. The state is the data we are manipulating. The reducer function receives an action, which is executed by a dispatch function".


### Sources :
[source1](https://gosink.in/react-js-how-to-render-useeffect-only-once/)

[source2](https://www.linkedin.com/pulse/provide-callback-usestate-hook-like-setstate-saransh-kataria/)
