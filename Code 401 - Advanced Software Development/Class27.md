# Class 27 Summary:

## Hook :

### How does React differ from vanilla JS/HTML/CSS?

  * Vanilla JS requires a lot of typing : JS requires a lot of codes so would be little messy and that make it less efficient than React.

  * React JS is for code organization :ReactJs is great for organizing the code. as you can see all the above code is on one page, script.js.

  *  "React :A JavaScript library for building user interfaces. Lots of people use React as the V in MVC. Since React makes no assumptions about the rest of your technology stack, it's easy to try it out on a small feature in an existing project".

  * "Vanilla.JS: A fast, lightweight and cross-platform framework. It is a fast and cross-platform framework for building incredible, powerful JavaScript applications. it is the most lightweight framework available anywhere".

### What is the primary difference between a function component and a class component?
 
  * "Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword".
  * "React lifecycle methods (for example, componentDidMount) cannot be used in functional components".
  * "There is no render method used in functional components".
  * "Functional components can accept and use props".
  * "Functional components should be favored if you do not need to make use of React state".

  * "Class components make use of ES6 class and extend the Component class in React".
  * "Sometimes called “smart” or “stateful” components as they tend to implement logic and state".
  * "React lifecycle methods can be used inside class components (for example, componentDidMount)".
  * "You pass props down to class components and access them with this.props".

### Document the following Vocabulary Terms:


| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|Functional Components  |are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword  |
|Children / Child Components  |Children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children  |


### Hooks :

  *  "Hooks are an experimental proposal to React. You don’t need to learn about them right now. Also, note that this post contains my personal opinions and doesn’t necessarily reflect the positions of the React team".

### Use Hooks :

  * "when we write a function component, and then we want to add some state to it, previously you do this by converting it to a class. But, now you can do it by using a Hook inside the existing function component".

### Using the State Hook :

  * " In a function component, we have no this, so we can’t assign or read this.state. Instead, we call the useState". 
  * " The only argument to the useState() Hook is the initial state. Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need".

![image3](https://user-images.githubusercontent.com/79833733/128629781-75dc71bc-9661-4345-bb84-3bf20c683c1b.png)

### Hooks at a Glance :

  * "Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes — they let you use React without classes. (We don’t recommend rewriting your existing components overnight but you can start using Hooks in the new ones if you’d like".

  * "React provides a few built-in Hooks like useState. You can also create your own Hooks to reuse stateful behavior between different components. We’ll look at the built-in Hooks first".

  * "The Effect Hook, useEffect, adds the ability to perform side effects from a function component.  It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes, but unified into a single API.".

  * "When we call useEffect, we’re telling React to run your “effect” function after flushing changes to the DOM. Effects are declared inside the component so they have access to its props and state. By default, React runs the effects after every render — including the first render".

### Hooks API Reference :
##### Basic Hooks
   * useState
   ![image1](https://user-images.githubusercontent.com/79833733/128629975-1d813dcd-8d83-4ccd-8cd0-aaf587e3ffb8.png)

   * useEffect
   ![image2](https://user-images.githubusercontent.com/79833733/128630148-7d17a135-2392-48e3-be89-c1e23c7e2df2.png)

   * useContext

##### Additional Hooks

  * useReducer
  * useCallback
  * useMemo
  * useRef
  * useImperativeHandle
  * useLayoutEffect
  * useDebugValue





### Sources : 

[source1](https://stackshare.io/stackups/react-vs-vanilla-js)

[source2](https://www.freecodecamp.org/news/functional-components-vs-class-components-in-react/)

[source3](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[source4](https://reactjs.org/docs/hooks-state.html)

[source5](https://reactjs.org/docs/hooks-overview.html)

[source6](https://reactjs.org/docs/hooks-reference.html)







