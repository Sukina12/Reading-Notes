# Class 13 Summary:

## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS :

* Cookies were invented early in the web’s history to be used for presistent local storage of small amount of data . But the negative aspects are:
1. Cookies included with every HTTP request : slowly down the web application by transmitting the same data over needlessly.
2. Cookies included with every HTTP request :sending data unencrypted over the internet.
3. Cookies limited at about 4 KB data, this slow the application.

* We need :
1. a lot of storage space.
2. on the client.
3. isn't transmitted to server.

#### Breif History Of Local Storage:

* Microsoft invented DHTML Brhaviors , one of them is (userData) which allws web pages to store up to 64 KB of data per domain.

* In 2002 Adobe introduced Flash 6 (Flash cookies) to store up to 100 KB of data per domain.

* In 2007 Google launched Gears which can store unlimited amounts of data per domain in SQL database tables.

#### HTML5 Storage:

* It's a way for web pages to store named key/value pairs locally, within the client web browser.

* From Java Script code , we will access HTML5 storage through the local storage object on the global window object.

#### Using HTML5 Storage:

* With web storage, web applications can store data locally within the user's browser.
* HTML5 Storage is based on named key/value pairs. 
* We will need to use functions like: parseInt() , parseFloat() , Calling getItem() , setItem()
* example:
![HTML storage](https://miro.medium.com/max/1134/1*OpOBcqJpawgs4ehT1eKZnA.png)

#### Tracking Changes To HTML5 Storage Area:

*example:
![storageevent](https://image.slidesharecdn.com/html5localstorage-140511235722-phpapp01/95/html5-local-storage-12-638.jpg?cb=1399852926)

#### HTML Web Storage Objects:

* HTML provides two objects for storing data :
1. Windows.localStorage (stores data with no expiration date)
2. windows.sessionStorage (stores data for one session)

** this information from  [web](http://diveinto.html5doctor.com/storage.html)

**Sukina AbuHammad**
