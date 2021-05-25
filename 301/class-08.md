## API Design Best Practices

Roy Fielding proposed **Representational State Transfer (REST)** as an architectural approach to designing web services. **REST is an architectural style for building distributed systems based on hypermedia**. REST is independent of any underlying protocol and is not necessarily tied to HTTP.

Most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

A primary advantage of REST over HTTP is that it uses open standards, and does not bind the implementation of the API or the client applications to any specific implementation. For example, a REST web service could be written in ASP.NET, and client applications can use any language or toolset that can generate HTTP requests and parse HTTP responses.

 -	REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

 -	A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be

 -	Clients interact with a service by exchanging representations of resources. Many web APIs use JSON as the exchange format.

 -	REST APIs use a uniform interface, which helps to decouple the client and service implementations. For REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources. The most common operations are GET, POST, PUT, PATCH, and DELETE.

Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid **"chatty" web APIs** that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.


### Define API operations in terms of HTTP methods

The HTTP protocol defines a number of methods that assign semantic meaning to a request. The common HTTP methods used by most RESTful web APIs are:

 -	**GET** retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.

 -	**POST** creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.

 -	**PUT** either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.

 -	**PATCH** performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.

 -	**DELETE** removes the resource at the specified URI.

**The differences between POST, PUT, and PATCH can be confusing.**
 -	POST request creates a resource. The server assigns a URI for the new resource, and returns that URI to the client. In the REST model, you frequently apply POST requests to collections. The new resource is added to the collection. A POST request can also be used to submit data for processing to an existing resource, without any new resource being created.

 -	A PUT request creates a resource or updates an existing resource. The client specifies the URI for the resource. The request body contains a complete representation of the resource. If a resource with this URI already exists, it is replaced. Otherwise a new resource is created, if the server supports doing so. PUT requests are most frequently applied to resources that are individual items, such as a specific customer, rather than collections. A server might support updates but not creation via PUT. Whether to support creation via PUT depends on whether the client can meaningfully assign a URI to a resource before it exists. If not, then use POST to create resources and PUT or PATCH to update.

 -	A PATCH request performs a partial update to an existing resource. The client specifies the URI for the resource. The request body specifies a set of changes to apply to the resource. This can be more efficient than using PUT, because the client only sends the changes, not the entire representation of the resource. Technically PATCH can also create a new resource (by specifying a set of updates to a "null" resource), if the server supports this.



Q1) What does REST stand for?<br>
Representational State Transfer (REST)

Q2) REST APIs are designed around a ____.<br>
resources

Q3) What is an identifer of a resource? Give an example.<br>
It is a URI that uniquely identifies that resource. As an example https://adventure-works.com/orders/1

Q4) What are the most common HTTP verbs?<br>
GET, POST, PUT, PATCH, and DELETE.

Q5) What should the URIs be based on?<br>
It is based on the Clients interact with a service by exchanging representations of resources.


Q6) Give an example of a good URI.<br>
https://adventure-works.com/customers/1/orders/99/products.<br>

Q7) What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?<br>
It exposes a large number of small resources; such an API may require a client application to send multiple requests to find all of the data that it requires. Which will all web requests impose a load on the web server

Q8) What status code does a successful GET request return?<br>
A successful GET method typically returns HTTP status code 200 (OK)

Q9) What status code does an unsuccessful GET request return?<br>
The method should return 404 (Not Found).


Q10) What status code does a successful POST request return?<br>
It returns HTTP status code 201 (Created).

Q11) What status code does a successful DELETE request return?<br>
The web server should return HTTP status code 204,


**Resources:**

[API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

