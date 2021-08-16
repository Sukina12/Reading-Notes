# Class 33 Summary:

## <Login /> and <Auth /> :

### Why is the Context API useful?

  * " because it can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props".

### Can a component outside of a provider get its context?

  * "No, it's need to be wrapped between the provider Tag".

### What are some common use cases for using the Context API?

  * "Change the profile data for the user to be access in any where inside the components and the theme ".

### Describe “Context Hell”?

  * " the React Context hell is the nasty code you get taking advantage of the React Context API".

### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|global state  |a set of local states which are all concurrent with each other. ... A global state in the time domain is also a global state in the causal domain |
|global context  | This is context that affects the entire application, and it will share data to everything in the React component tree. |
|provider  |	The context provider accepts a value that will be passed to its children. All children components will re-render when the value changes. |
|consumer  |This is a React component that subscribes to context changes in value of the Provider. |

### What is Role-Based Access Control (RBAC)?

#### DEFINITION OF ROLE-BASED ACCESS CONTROL (RBAC) : 
  * "Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network".

#### Some of the designations in an RBAC tool can include:
  1. Management role scope : it limits what objects the role group is allowed to manage.
  2. Management role group : you can add and remove members.
  3. Management role : these are the types of tasks that can be performed by a specific role group.
  4. Management role assignment  : this links a role to a role group.

#### BENEFITS OF RBAC :
  1. Reducing administrative work and IT support
  2. Maximizing operational efficiency
  3. Improving compliance

#### React-cookies :

  * "Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them".

  * To set or remove the cookies, we are using a third-party dependency of react-cookie

  * Install : npm i react-cookies

  * "To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie".

#### Sources:
[source1](https://dev.to/alfredosalzillo/the-react-context-hell-7p4)
[source2](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)
[source3](https://www.npmjs.com/package/react-cookies)

