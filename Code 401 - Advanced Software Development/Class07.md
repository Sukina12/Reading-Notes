# Class 07 Summary :

### Bearer Authorization :

### Write the following steps in the correct order :

  1. Register your application to get a client_id and client_secret.
  2. Ask the client if they want to sign in via a third party.
  3. Redirect to a third party authentication endpoint.
  4. Make a request to a third-party API endpoint
  5. Receive authorization code.
  6. Make a request to the access token endpoint.
  7. Receive access token

### What can you do with an authorization code?

  * For Authorization Code grant type, the first step is to issue an auth code to the client. The client will then get back with the auth code and client credentials to request for a token.

### What can you do with an access token?

  *  it will include that token as a credential when making API requests. To do so, it should transmit the access token to the API as a Bearer credential in an HTTP Authorization header.

### What’s a benefit of using OAuth instead of your own basic authentication?

  1. It allows you to read data of a user from another application.
  2. It supplies the authorization workflow for web, desktop applications, and mobile devices.
  3. Is a server side web app that uses authorization code and does not interact with user credentials.
  4. It gives users more control over their data; they can selectively grant access to various functionalities for applications they want to use.


| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| Client ID | is a public identifier for apps. Even though it’s public, it’s best that it isn’t guessable by third parties, so many implementations use something like a 32-character hex string.|
| Client Secret |  is a secret known only to the application and the authorization server. |
| Authentication Endpoint  | Use the authentication endpoint to specify an endpoint that is called to obtain an access token which can then be used in the subsequent password update callouts.  |
| Access Token Endpoint | A token endpoint is an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.  |
| API Endpoint    |  is one end of a communication channel. When an API interacts with another system, the touchpoints of this communication are considered endpoints. For APIs, an endpoint can include a URL of a server or service.  |
| Authorization Code    |  is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.   |
| Access Token    | are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data.  |

### What is JSON Web Token?

  *  "is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed".

### When should you use JSON Web Tokens? 
  
  1. Authorization
  2. Information Exchange

### What is the JSON Web Token structure?

   1. Header
   2. Payload
   3. Signature

![Example](https://res.cloudinary.com/practicaldev/image/fetch/s--VEc3u5IA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/xdc4axtmpwsut743q2s2.png)


### Sources:

[source1](https://auth0.com/docs/tokens/access-tokens/use-access-tokens)

[source2](https://www.clowder.com/post/why-your-organization-should-be-using-oauth-2.0)

[source3](https://www.oauth.com/oauth2-servers/access-tokens/)

[source4](https://jwt.io/introduction/)






