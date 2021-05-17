# Class 13 summary:

### CRUD:

* 100’s = informational status response code indicates that everything so far is OK and that the client should continue with the request or ignore it if it is already finished.

* 200’s = success status response code indicates that the request has succeeded. 

* 300’s = Multiple Choices redirect status response code indicates that the request has more than one possible responses.

* 400’s = Bad Request response status code indicates that the server cannot or will not process the request due to something that is perceived to be a client error

* 500’s =  caused by an error during the execution of any policy within Edge or by an error on the target/backend server.

![STATUS](https://allprowebdesigns.com/blog/wp-content/uploads/2019/10/status-codes-638x445.jpg)

* 200 OK : response status code indicates that the request has been accepted for processing, but the processing has not been completed.

* 308 : Permanent Redirect --> redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers.

* 204 No Content  --> code for updates that don’t return data to the client.

* 414 URI Too Long response status code indicates that the URI requested by the client is longer than the server is willing to interpret.

* The HTTP 403 Forbidden client error status response code indicates that the server understood the request but refuses to authorize it.

![CRUD](https://miro.medium.com/max/768/1*D07GoP9ZO3rXSVsVndX5kg.png)

**************************************************************************************************************************

### REST:

* Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

* app.use(express.json()): is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application.

* /project/:id path ---> This means the component will see the dynamic part in the id parameter.

* The  difference between the (PUT) and (PATCH) method ---> PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, But PATCH method supplies a set of instructions to modify the resource.

*  (HTTP) 500 Internal Server Error----> server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. 

*  The 200 status --->  the most common returned. It means that the request was received and understood and is being processed. A 201 status code---> indicates that a request was successful and as a result, a resource has been created.

![REST](https://images.tutorialedge.net/uploads/rest-api.png)

*************************************************************************************************************************

* Sources:

* [source1](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

