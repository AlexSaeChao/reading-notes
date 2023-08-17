# Reading 29

Reading 29 delves into using Room in Android for data tasks like CRUD operations. It also compares Room's features with JPA, emphasizing shared methods like annotations and the DAO pattern. Through examples and analogies, it clarifies the connection between Room, SQLite, and JPA.

## Data and Entity with Room

What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?

The database engine that Room is wrapped with is called SQLite.

> The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite. In particular, Room offers:
> - Compile-time verification of SQL queries.
> - Convenience annotations that reduce repetitive and error-prone boilerplate code.
> - Streamlined database migration paths.
>
> Given these considerations, it is highly recommended to use Room over the SQLite APIs directly.

Do Rooms have any similarities to JPA?

Yes, Room and JPA (Java Persistence API) have the following similarities:

- **Annotation-based Mapping**: Both Room and JPA use annotations to define entities and map them to database tables. In Room, the `@Entity` annotation is used to define a table, akin to JPA's `@Entity`.
  
- **DAO Pattern**: Both Room and JPA utilize the Data Access Object (DAO) pattern, allowing for a clean separation of CRUD operations from the database.
  
- **Relationship Handling**: Both frameworks offer ways to handle database relationships (e.g., one-to-one, one-to-many) using annotations.

Describe a DAO in your own words

I'll describe it with an anology.

Imagine a library with access to a vast collection of books, organized in various sections, shelves, and racks. If a student needs a book, they can seek assistance from the librarian, who acts as an intermediary. The librarian fetches the requested book or accepts returns, sparing the student the task of navigating the library's intricacies.

In this analogy:

- The **library** represents the database with all its complexities.
- The **books** symbolize data or records in the database.
- The **librarian** signifies the DAO.

Just as you communicate with the library (database) through the librarian (DAO) to borrow or return books (data), in software development, the application interacts with the database through the DAO to fetch, insert, update, or delete records. The DAO abstracts away the intricacies of the database and provides a simple and consistent interface to interact with the data.

## Things I want to know more about

## References

[Overview: Saving data with Room](https://developer.android.com/training/data-storage/room)

[Defining entities in Room](https://developer.android.com/training/data-storage/room/defining-data)

[Related entities in Room](https://developer.android.com/training/data-storage/room/relationships)

[Accessing data with Room](https://developer.android.com/training/data-storage/room)
