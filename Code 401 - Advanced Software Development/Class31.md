# Class 31 Summary:

## Context API

### Describe use cases useState() vs useReducer() ?

  * "useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState".
  * "useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks".

### Why do custom hooks need the use prefix?

  * "The name of any custom hook should begin with use. This convention indicates to developers that hooks are used within the file/custom hook".

### What do custom hooks usually do?

  * " Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks".

### Using any list of custom hooks, research and name one that you think will be useful in your applications?

  1. "useScript React hook to dynamically load an external script and know when its loaded ,useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically".

  2. use-mouse-action :"A library with three React hooks for listening to mouse events on an element or JSX element. useMouseAction: This is used to register mouse actions on an element. useMouseDown: This is used to register a mouse down event on an element. useMouseUp: This registers a mouse up event on an element".

### Describe how a hook that fetches API data might work?

  * "The hook might take in a url, a method, and a body. Using axios or something similar, useState and possibly useEffect, an API call can be made based on and using the parameters passed in and then an objects state could be ‘set’ based on the results of the API call".

### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|reducer |Reducers in NgRx are responsible for handling transitions from one state to the next state in your application. Reducer functions handle these transitions by determining which actions to handle based on the action's type   |


### Context :

#### When to Use Context :
  
  * "Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language".

![image1](https://user-images.githubusercontent.com/79833733/129165941-3c7ce36b-ce69-4206-a0ea-fa38d5575e68.png)

#### Before You Use Context :

  * "Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult".

  * "If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context".

#### React.createContext :

  * "Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree".

#### Context.Provider:

  * "Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes".
  * "The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree".

#### Class.contextType :

  * "The contextType property on a class can be assigned a Context object created by React.createContext()". 

#### Context.Consumer :

  * "A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component".

#### Caveats:
 
  * "Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders".

### An Exercise in Hooks and Context:

  * "After performing an audit on how we communicate with our users, we landed with a simple system of three classes of communication, and snackbars fit perfectly on the ‘low priority’ end of that spectrum. They are small notifications that show up on the screen when a user performs an action. They are not intrusive at all and appear for just a brief moment".

#### Sources:
[source1](https://dev.to/spukas/3-reasons-to-usereducer-over-usestate-43ad)
[source2](https://www.wix.engineering/post/custom-react-hook-when-software-design-meets-react-hooks)
[source3](https://ngrx.io/guide/store/reducers)
[source4](https://reactjs.org/docs/context.html)
[source5](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)




