# Class 11 Summary

###  Authentication:

* Authentication is the process of recognizing a user’s identity.The authentication process always runs at the start of the application, and before any other code is allowed to proceed. 

* Example Of Authentication : Netlify & Heraku

* Authentication steps to work:
1. "The two websites connect to each other using Auth0".
2. "The second site generate 1-time token & 1-time secret unique".
3. "The first site give the token and the secret".
4. "The authorization provider take the request from the client software".
5. "if there is no Authentication , the client ask for Authentication and get the approve".
6. "the users approve on transaction".
7. "The user is given an approved access token".
8. "the user see successfull completed transaction".

* OpenID : allow you to use an existing account to sign in to multiple websites, without needing to create new passwords.

****************************************************************************************************

### Authentication and Authorization Flow:

* Authentication means confirming your own identity, while authorization means granting access to the system. Authentication is the process of verifying who you are, while authorization is the process of verifying what you have access to.


* "Authorization code flow is used to obtain an access token to authorize API requests. Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API".


* Authorization Code Flow with Proof Key for Code Exchange (PKCE) is a security extension to OAuth for public clients on mobile devices, designed to prevent interception of the authorisation code by a malicious application that has sneaked into the same device.


* Implicit Flow with Form Post : applies to traditional web apps as opposed to SPAs. You obtain ID tokens as opposed to access tokens, which have a completely different intended use. 


* client credentials flow, permissions are granted directly to the application itself by an administrator. When the app presents a token to a resource, the resource enforces that the app itself has authorization to perform an action since there is no user involved in the authentication.

* Resource Owner Password Flow : exchanging the username and password of a user for an access token and, optionally, a refresh token. ... The primary difference is that the user's password is accessible to the application. This requires strong trust of the application by the user.

[img](https://www.oreilly.com/library/view/getting-started-with/9781449317843/httpatomoreillycomsourceoreillyimages986441.png)

*****************************************************************************************************

* Sources : 

* [source1](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

* [source2](https://auth0.com/docs/flows)


