# More CRUD

This sections talks about more CRUD basics and creating a Restful API. These steps provide a general overview of creating a RESTful API, but the specifics may vary depending on the frameworks, libraries, and databases used, as well as the requirements of your API.

## CRUD Basics

Which HTTP method would you use to update a record through an API?

> You can create something new, read or view the newly created data, edit or update the data and finally the option to delete it.

Put is the HTTP Method to use to updat a record through an API

Which REST methods require an ID parameter?

Update and Delete requires an ID parameter.

## Speed Coding: Building a CRUD API

What’s the relationship between REST and CRUD?

REST and CRUD can do similar things but REST is an arcitectual style that can be used to design APIs, and CRUD represents what you could do (the basic operations that can be performed on a data within a system).

If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

1. Set up server
    * npm install express
2. Define the Routes
    * defines the routes for CRUD Ops, like endpoints
3. Mount the router
    * Mount the router inside the API
4. Connect to a Database
    * like mongoDB and define the collections
5. Implement CRUD Functionality
    * Handle incoming requests and validate input data, using appropriate methods. then finally handle errors

## Things I want to know more about

Seems like creating a RESTful API is one of newer standards in the industry, whats the importance of working with a non RESTful API with legacy systems and can they reworked or refactored into something more RESTful?

## References

[CRUD Operations Explained](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

[Speed Coding: Building a CRUD API (Watch a Twitch streamer code an Express API in 20 minutes!)](https://www.youtube.com/watch?v=EzNcBhSv1Wo)