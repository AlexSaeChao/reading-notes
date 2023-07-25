# Reading 12

## Spring guide: Accessing Data with JPA

How are query methods defined when using Spring Data JPA?

Which dependencies will you need in order to complete the Spring guide?

`spring-boot-starter-data-jpa`
`spring-boot-starter-web`

What annotations are used to specify an auto generated identification number for an Entity?

```java
package com.example.accessingdatajpa;

import jakarta.persistence.Entity;
import jakarta.persistence.GeneratedValue;
import jakarta.persistence.GenerationType;
import jakarta.persistence.Id;

@Entity
public class Customer {

  @Id
  @GeneratedValue(strategy=GenerationType.AUTO)
  private Long id;
  private String firstName;
  private String lastName;

  protected Customer() {}

  public Customer(String firstName, String lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
  }

  @Override
  public String toString() {
    return String.format(
        "Customer[id=%d, firstName='%s', lastName='%s']",
        id, firstName, lastName);
  }

  public Long getId() {
    return id;
  }

  public String getFirstName() {
    return firstName;
  }

  public String getLastName() {
    return lastName;
  }
}
```

> Here you have a `Customer` class with three attributes: `id`, `firstName`, and `lastName`. You also have two constructors. The default constructor exists only for the sake of JPA. You do not use it directly, so it is designated as `protected`. The other constructor is the one you use to create instances of `Customer` to be saved to the database.
> The `Customer` class is annotated with `@Entity`, indicating that it is a JPA entity. (Because no `@Table` annotation exists, it is assumed that this entity is mapped to a table named `Customer`.)
> The `Customer` object’s `id` property is annotated with `@Id` so that JPA recognizes it as the object’s ID. The `id` property is also annotated with `@GeneratedValue` to indicate that the ID should be generated automatically.
> The other two properties, `firstName` and `lastName`, are left unannotated. It is assumed that they are mapped to columns that share the same names as the properties themselves.
>The convenient `toString()` method print outs the customer’s properties.

## Baeldung: Comparing repositories (we’ll be using JpaRepository)

Which of the Spring Data Repositories covered in the readings has the most methods available to it?

The `JpaRepository` has the most methods available to it. `JpaRepository` extends `PagingAndSortingRepository`, which in turn extends `CrudRepository`

Name a downstide of a Spring Data Repository.

> Beyond all the very useful advantages of these repositories, there are some basic downsides of directly depending on these as well:
> * We couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; that's, of course, not unique to this library – but we do have to be careful not to expose these internal implementation details
> * By extending, e.g. CrudRepository, we expose a complete set of persistence methods at once. This is probably fine in most circumstances as well, but we might run into situations where we'd like to gain more fine-grained control over the methods exposed, e.g. to create a ReadOnlyRepository that doesn't include the save(…) and delete(…) methods of CrudRepository

How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

```java

public interface StudentRepository extends JpaRepository<Student, Long> {
    List<Student> findByName(String name);
}
```

## Things I want to know more about

JPA feels like Java with SQL capabilities.

## References

[Spring guide: Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)

[Baeldung: Comparing repositories (we’ll be using JpaRepository)](https://www.baeldung.com/spring-data-repositories)