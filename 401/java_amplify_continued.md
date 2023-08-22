# Reading 32

The document discusses what makes an API RESTful, the benefits of GraphQL and an explaination on what is serverless.

## Java Amplify Continued

What makes an API RESTful?

What makes an API RESTful is clear seperation between client and server. They are stateless and cacheable, meaning each request from a slient has all the information the server needs to understand and respond to all the while not retaining an session info.

What is the benefit of using GraphQL? Any downsides?

- **Pros**
  - flexible queries
  - Using a single endpoint for all of it's interaction
  - Strongly or strictly typed schema serving a contract between client and server, make it clear what kind of data to expect.

- **Cons**
  - Not justified for all use case, like when using a simple API.
  - Kind of complex making caching more challenging that standard URL based caching in REST.

Describe “serverless” to a new 301 Code Fellows student.

ALright I'm going to go with an analogy to explain serverless.

- Imagine you live in Seattle and need to get around town. You have two main options: buying or renting a car (similar to traditional servers) or using public transportation (akin to being serverless).

- **Owning/Renting a Car (Traditional Servers):**
You have the initial cost of purchasing or renting the car.
Maintenance, fuel, and repairs come out of your pocket, much like the upkeep for a dedicated server.
Regardless of the city's events or traffic changes, you're limited to the capacity of your car. If you need more space for people or items, you're out of luck unless you invest in a bigger vehicle.

- **Public Transportation (Serverless):**
Instead of a hefty initial purchase, you pay per ride, just like you'd pay for the compute time you use in a serverless model.
The city (or cloud provider, in the case of serverless) handles all operational and maintenance costs.
No worries about parking, insurance, or upkeep.
During large city events, the transportation system can add more buses or trains to meet the increased demand, similar to how serverless platforms automatically scale resources.

## Things I want to know more about

## References

[Intro to Serverless](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

[AWS Amplify](https://aws.amazon.com/amplify/)

[GraphQL Intro (just read the first few paragraphs, up until the query code)](https://docs.amplify.aws/cli/graphql/data-modeling/)
