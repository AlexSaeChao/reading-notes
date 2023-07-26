# Reading 13

## Related data in Spring (only read section “3. One-to-Many Relationship”)

Name a few real life examples of “One To Many” relatioships.

* Team and Players
* Parent and child
* Books and pages
* Author and Books
* Customer and Orders

Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

The Player would be the many and the Team would be considered the one.

Explain one to many relationships to a non-technical friend.

Think of a family tree with multiple children to one set of parents. One set of parents can have any number of children but one child can only have one set of parents. These relationships may not necessarily need to be derived directly from one another, like parent and children, in a learning environment you may have teachers(one) and students(many). As long as there is an entity of one connected to an entity of any number, and that relationship can't be reversed in normal circumstances.

## Baeldung: Spring Integration Testing

Describe the difference between a unit test and an integration test.

Unit tests are usualy done for individual components to test if the behave and performs as expected in isolation.
Integration tests cover multiple units, used to test if different parts of the application can perform as intended together.

What is the object that provides support for Spring MVC Testing?

> MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

What does the “perform()” method do in a Spring integration test?

In Spring integration tests using MockMvc, the `perform()` method is used to perform a mock HTTP request to a specific endpoint/route.

## Things I want to know more about

## References

[Related data in Spring (only read section “3. One-to-Many Relationship”)](https://www.baeldung.com/spring-data-rest-relationships)

[Baeldung: Spring Integration Testing](https://www.baeldung.com/integration-testing-in-spring)