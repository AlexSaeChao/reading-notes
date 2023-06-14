# API Design Best Practices

Best practices for designing RESTful web APIs. This reading covers various aspects such as the definition of REST, the use of resources and identifiers, the importance of using appropriate HTTP verbs, guidelines for URI design, the impact of "chatty" APIs, and the significance of HTTP status codes in different types of requests. It emphasizes designing APIs that are efficient, adhere to REST principles, and provide a good user experience.

What does REST stand for?

Rest stands for Representational State Transfer

REST APIs are designed around a ____.

> REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

What is an identifier of a resource? Give an example.

> A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

```http

https://adventure-works.com/orders/1

```

What are the most common HTTP verbs?

> REST APIs use a uniform interface, which helps to decouple the client and service implementations. For REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources. The most common operations are GET, POST, PUT, PATCH, and DELETE.

What should the URIs be based on?

> When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

Give an example of a good URI.

``` http

https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid

```

What does it mean to have a ‘chatty’ web API?

> Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.

Is this a good or a bad thing?

I'd say it's a bad thing to have a chatty API, fetching data the client doesn't need will increase latency and probably use up more bandwidth.

What status code does a successful GET request return?

> A successful GET method typically returns HTTP status code 200 (OK).

What status code does an unsuccessful GET request return?

> If the request was fulfilled but there is no response body included in the HTTP response, then it should return HTTP status code 204 (No Content)

What status code does a successful POST request return?

> If a POST method creates a new resource, it returns HTTP status code 201 (Created)... Alternatively, if there is no result to return, the method can return HTTP status code 204 (No Content) with no response body.

What status code does a successful DELETE request return?

> If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information. If the resource doesn't exist, the web server can return HTTP 404 (Not Found).

## Things I want to know more about

Are there any use cases to use verbs in URIs that may be justifed?

Are there any best practices for error handling and returning the appropriate status codes?

## References

[RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)
