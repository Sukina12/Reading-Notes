# Class 28 Summary :

##  Component Lifecycle / useEffect() :

### Why do we not need more .html pages in a multi-page React app?
  * In Multi-page apps, we get back multiple HTML pages, where each page has content for given Router.
  * In Multi-page apps, we only use React to create widgets.
  * In the Multipage apps, we split up our components but a lot of pages are going to be normal HTML pages, and widgets we dump in like an Image gallery that is managed by React, so the entire page is not under React control.
  * Because we build a react frontend client side that is a Single page Application, it's rendering the component that will render on the page not by render a new page.

### If we wanted a component to show up on every page, where would we put it and why?

  * Inside the <BrowserRouter />, outside a <Route />

### What does routing do with the components that were rendered when a new route is requested?

  * It renders the appropriate user interface when the current location matches the route’s path. 
  * The component prop defines the React element that will be returned by the Route when the path is matched. This React element is created from the provided component using React.createElement.

### What does props.children contain?

  * children is a special property of React components which contains any child elements defined within the component, e.g. the divs inside Example above. {this.props.children} includes those children in the rendered result.

### How do useState() and this.setState() differ?

  * The setState function is used to handle the state object in a React class component. 
  * setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

### Document the following Vocabulary Terms:

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|State Hook |the State of a component is an object that holds some information that may change over the lifetime of the component.and  Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.  |
|Mounting and Un-Mounting |Mounting is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components). & Un-Mounting: This method is called just before the component gets destroyed. Any clean up statements should be executed inside this method. |


### Effect Hook :

  * "By using useEffect, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API".

  ![image1](https://user-images.githubusercontent.com/79833733/128691031-8aa42add-1a4f-4741-9803-991429aa4755.png)

  * " Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope". 

  * "React performs the cleanup when the component unmounts. However, effects run for every render and not just once. This is why React also cleans up effects from the previous render before running the effects next time".



### Sources :

[source1](https://morioh.com/p/1e31a980e5a6)

[source2](https://medium.com/the-andela-way/understanding-the-fundamentals-of-routing-in-react-b29f806b157e)

[source3](https://stackoverflow.com/questions/49706823/what-is-this-props-children-and-when-you-should-use-it)

[source4](https://stackoverflow.com/questions/61574982/what-is-the-difference-between-react-setstate-and-hooks-setstate)

[source5](https://reactjs.org/docs/hooks-effect.html)


