# Reading 33

## GraphQL Relationships & Completable Future

Describe asynchronous actions in your own words.

An asynchronous action refers to a task or operation that runs separately from the main flow of a program, allowing the program to continue its execution without waiting for the asynchronous task to complete. It's like starting a laundry cycle and then cooking dinner; you don't need to wait for the laundry to finish to start cooking. Both tasks happen independently of each other.

Later on, once the asynchronous operation finishes, a callback function or some other mechanism like a promise or future is triggered, indicating the result of the operation or that a particular task is complete.

So let's say your main flow was to cook dinner, you would run your laundry first and then commence with the cooking, when the laundry cycle is complete, it alert you with beeps.

What is the benefit of asynchronous methods?

- By using the Completable Future, developers can write non-blocking code. This allows the system to remain responsive even when performing lengthy or resource-intensive tasks.

- You can combine multiple CompletableFuture objects allows for parallel execution of tasks

## Things I want to know more about

What's the Difference Between Multithreading and Asynchrony?

What Are Race Conditions and How Do They Happen?

Callback hell..

## References

[One-to-many and many-to-one connections using GraphQL in AWS Amplify](https://docs.amplify.aws/cli/graphql/data-modeling/#has-many-relationship) (only read the “Has Many relationship” section)

[CompletableFuture in Java](https://www.baeldung.com/java-completablefuture) (only read through section 3)
