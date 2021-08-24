# Class 39 Summary:

##  Redux - Additional Topics :

### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

  * "use redux-thunk and mapDispatchToProps to inject fetchDepartments to the stateless component and implement componentWillMount or similar lifecycle method, to load data - but then I don't need to pass the list via props, as the component would always load data for himself, and I don't want that, because whenever a new component is created the data is fetched from api instead of store".

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

  * "When the asynchronous task ends, a callback should manage the outcome of the asynchronous task and appropriately update the state with a positive or negative response, support asynchronous actions by modifying their reducers, i.e. making sure that the reducer intercepting that action starts the asynchronous task and manages its outcome".

### Document the following Vocabulary Terms :  

| Term      |                                                   |
| -----------  | ----------------------------------------------------------------|
|middleware |software that enables one or more kinds of communication or connectivity between two or more applications or application components in a distributed network |
|thunk |a subroutine used to inject a calculation into another subroutine. Thunks are primarily used to delay a calculation until its result is needed, or to insert operations at the beginning or end of the other subroutine |

### Redux Toolkit :
   * The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:
     1. "Configuring a Redux store is too complicated".
     2. "I have to add a lot of packages to get Redux to do anything useful".
     3. "Redux requires too much boilerplate code".
  
   * "Redux Toolkit also includes a powerful data fetching and caching capability that we've dubbed "RTK Query". It's included in the package as a separate set of entry points. It's optional, but can eliminate the need to hand-write data fetching logic yourself".

   * "Redux Toolkit is available as a package on NPM for use with a module bundler or in a Node application :
       ** npm install @reduxjs/toolkit

   * Redux Toolkit includes these APIs :
      1. configureStore(): wraps createStore to provide simplified configuration options and good defaults.
      2. createReducer(): that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements.
      3. createAction(): generates an action creator function for the given action type string.
      4. createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.
      5. createAsyncThunk: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise
      6. createEntityAdapter: generates a set of reusable reducers and selectors to manage normalized data in the store
      7. The createSelector utility from the Reselect library, re-exported for ease of use.

### RTK Query :
   * "RTK Query is provided as an optional addon within the @reduxjs/toolkit package. It is purpose-built to solve the use case of data fetching and caching, supplying a compact, but powerful toolset to define an API interface layer for your app".
  

#### Sources:
[source1](http://5.9.10.113/39356517/correct-way-to-pre-load-component-data-in-reactredux)
[source2](https://blog.logrocket.com/managing-asynchronous-actions-in-redux-1bc7d28a00c6/)
[source3](https://redux-toolkit.js.org/introduction/getting-started)