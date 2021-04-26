# Class 02 Notes

### State and Lifecycle

### Converting a Function to a Class:

* To convert function to a class, follow these steps:
1. create the class with the same name , that extends React Component.
2. Add single empty method to the function
3. move the function body into the method.
4. replace props whit this .props in the method body.
5. delete the empty function.

### Adding Local State to a Class:

1. replace this.props whith this.state.date in the method.
2. add a class constructor to assign the this.state initial.
3. remove the data props from the element.

![Example](https://www.codegrepper.com/codeimages/react-function-component-to-class-component.png)


### Handling Events:

* Handling event with React is similar to handeling event in DOM elements. with some syntax differences :
1. React camels named by using  camelCase instead of lowercase.
2. in JSX we pass function as the event hamdler rather than a string.

### Passing Arguments to Event Handlers:

* Inside a loop, if we want to pass an extra parameter to an event handler. 

![HandlingEvent](https://www.codevoila.com/cvuploads/images/201607/reactjs_component_event_handler.png)

### Conditional Rendering:

* in React we can create distinct components that encapsulate behavior which we need. After that , we can render only some of the components, depending on the state of our application.

* Conditional rendering in React Use if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

### Element Variables 

* We can use variables to store elements. This can help us conditionally render a part of the component while the rest of the output doesn’t change.

### Preventing Component from Rendering:

* if we  want a component to hide itself even though it was rendered by another component. return null instead of its render output.

* Returning null from a component’s render method does not affect the firing of the component’s lifecycle methods. For instance componentDidUpdate will still be called.


###### The Sorces:
[state-and-lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

[handling-events](https://reactjs.org/docs/handling-events.html)

[conditional-rendering](https://reactjs.org/docs/conditional-rendering.html)