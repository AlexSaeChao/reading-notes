# CRUD

Status codes and Building a Rest API

## Status Codes Based On REST Methods

In your own words, describe what each group of status code represents:

* 100’s = Informational, server has recieved the client's request and is in progress of processing it
* 200’s = Success in receiving and processed by the server
* 300’s = Redirection - the expected location may have move.
* 400’s = Client Error - client is
* 500’s = Server Error

What is a status code 202?

Normally used for asynch operations. The request has been accepted for processing but is not fully complete but it will be completed in the future.

What is a status code 308?

For permanent redirects. This code indecates that the requested resourse has been permanently moved to a different URL

What code would you use if an update didn’t return data to a client?

> 204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

What code would you use if a resource used to exist but no longer does?

> 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

What is the ‘Forbidden’ status code?

> 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


# Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

Why do we need to pull our MongoDB database string out of our server and put it into our .env?

For security reasons, the help prevent unauthorize usages and access to sensitive data.
For the flexibilty to change the database config without changing the code.

What is middleware?

Acts a bridge for between incoming requests and the server's response.

What does app.use(express.json()) do?

Function is a middleware in Express.js that enables the server to parse incoming requests with JSON payloads.

What does the /:id mean in a route?

It's a parameter, that we can access to route handle request for different users.

What is the difference between PUT and PATCH?

Put is completely moving the resources at a given URL, for updating or replacing the entire resource. While patching is used to modify parts of the fields or props.

How do you make a default value in a schema?

You can specify default prop when defining a field in the schema definition.

``` javascript

const userStuff = new Schema({
  name: {
    type: String,
    default: 'Anon',
  },
});

```

What does a 500 error status code mean?

It means that something went wrong on the server's side while processing the request, and it is unable to fulfill the request. Could be a server crash, unhandled exception or just something not wired correctly.

What is the difference between a status 200 and a status 201?

Both are successfull in the server recieving their requests but 200 has returned it as well. for 201 the request has made a new resource on the server as a result.

## Things I want to know more about

I would like to see each status code being used in a use case scenario and how to rememdy it if needed.

## References
[Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)