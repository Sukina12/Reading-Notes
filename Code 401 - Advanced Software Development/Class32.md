# Class 32 Summary:

##  Context API - Behaviors :

### When you have multiple contexts, what component type should you use (class/function) and why?

  * function, If two or more context values are often used together, you might want to consider creating your own render prop component that provides both.

### What are some good use cases for using the Context API for global state?

  1. Twilio : Twilio really defines what it means to be API-driven.
  2. Stripe : Stripe is one of the most successful and best known API-driven businesses.
  3. Ebay : Unlike the previous companies, eBay didn’t start out with the intent of being API-driven.
  4. Salesforce : XML APIs have been a part of Salesforce since day one, back in 2000 when it launched.
  5. Rovi :Rovi is definitely the oldest company on the list, founded as Macrovision in 1983.


### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| context | a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree |
|useContext()  | create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level  |
|static context  |which wraps our component with PureComponent shallow comparison logic while also allowing us to pass references from our context  |

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

#### Sources :
[source1](https://reactjs.org/docs/context.html)
[sourcse2](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
