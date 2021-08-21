# Class 36 Summary :

## Application State with Redux :

### What are the advantages of storing tokens in “Cookies” vs “Local Storage” ?

  * "Cookies are automatically saved, sent and removed by the browser. The frontend developer does not have to worry about implementing this part, nor is there any scope of a mistake from the frontend side. This is not true for localstorage".
  * "for API calls to the server, they will only get the session tokens if they are using cookies – localstorage will not work".
  * "The objective here is that the user should use the same session when navigating to different subdomains of a site. This can be easily done via cookies by setting the cookie domain as “.yoursite.com”.
  This is not easily possible to do via localstorage since the store is not shared across domains / subdomains".

### Explain 3rd party cookies :

  * "A third-party cookie is placed on a website by someone other than the owner (a third party) and collects user data for the third party. As with standard cookies, third-party cookies are placed so that a site can remember something about the user at a later time. Third-party cookies, however, are often set by advertising networks that a site may subscribe to in the hopes of driving up sales or page hits".

### How do pixel tags work?

  * "It’s a 1×1-pixel graphic used for tracking user behavior, site conversions, web traffic, and other metrics at a site’s server level. In other words, it is a tiny pixel-sized image, usually hidden, embedded in everything, from banner ads to emails".
  * "You add the tracking pixel using a code in your site’s HTML code or email, which contains an external link to the pixel server. When someone visits your website, the HTML code is processed by their browser, which follows the link and opens the hidden graphic. This action is identified and recorded in the server’s log files. This method allows for different information about the visitor to be transmitted".

### Document the following Vocabulary Terms :  

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|cookies | Cookies are data, stored in small text files, on your computer.When a web server has sent a web page to a browser, the connection is shut down, and the server forgets everything about the user. |
|authorization | the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular. More formally, "to authorize" is to define an access policy  |
|access control | is a security technique that regulates who or what can view or use resources in a computing environment  |
|conditional rendering | the process of delivering elements and components based on certain conditions. |

### Fundamentals of Redux :

  * "State management is absolutely critical in providing users with a well-crafted experience with minimal bugs".

  * "Redux provides a solid, stable, and mature solution to managing state in your React application".

  * "Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse".

  * "Redux is a predictable state container for JavaScript apps".

  * "It helps you write applications that behave consistently".

### What is Redux?
  * Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments and are easy to test.

### Why use Redux?
  * "Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app".

### how to use Redux in react
   1. create store as we create context
   2. pass store and context to provider
   3. imported as context exactly

### How Redux works
  * "There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another".

  * "There are three building parts: actions, store, and reducers".     
 

#### Sources :
[source1](https://supertokens.io/blog/cookies-vs-localstorage-for-sessions-everything-you-need-to-know)
[source2](https://whatis.techtarget.com/definition/third-party-cookie)
[source3](https://whatagraph.com/blog/articles/tracking-pixel)
[source4](https://egghead.io/courses/react-state-management-in-2021-6732)
[source5](https://blog.logrocket.com/why-use-redux-reasons-with-clear-examples-d21bffd5835/)

