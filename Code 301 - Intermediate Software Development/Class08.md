# Class 08 Summary:

### REST

* REST (Representational state transfer) : architectural software for styling web.used to create interactive application. it is independent of any protocol.

* REST APIs are designed around a resources (object, data or service).

* Identifier which the resource has is a unique URL that identifies the resource.
  
  example : HTTP "(https://adventure-works.com/orders/1)"

* HTTPverbs:
1. POST (create)
2. GET  (read)
3. PUT  (update/replace)
4. PATCH(update/modify)
5. DELETE(delete)

* URL (Uniform Resource Identifier) : sequence of characters  that identifies resource .  based standards on resource(nouns ) and the operation of the resource (not verbs).

* example of Good URL : https://adventure-works.com/orders 

* 'Chatty' web API : if designed the wrong resources for clients . and it is bad thing to make large number of small resources.

* Successful Get request return : HTTP code 200 (ok).

* Unsuccessful Get request return : HTTP code 400 (not found).

* Successful POST request return : HTTP code 201 (created). code 204 (no content).

* Successful DELETE request return : HTTP code 204 (accepted) . code 404 (not found).


************************************************************************************************************************************************

* sources:

[source 1](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)