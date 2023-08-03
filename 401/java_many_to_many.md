# reading 18

## Many to many relationships


Name a few examples of real world ManyToMany relationships.

* Tags and Posts
* Authors and Books
* Actors and Movies

Explain the significance of a join table for ManyToMany relationships.

A join table is like a bridge between the two groups in a many-to-many relationship. It helps connect them without repeating information.

What are the values held within a join table?

For example, in the "Students and Courses" example, the join table would have two columns: one for the student ID and one for the course ID.
Each row in the join table represents a connection between a specific student and a specific course. The values in the join table are the actual IDs (or primary keys) of the records from the related tables.

## Security: a humorous overview

According to the author of the article, will you ever be truly secure from ALL possible security threats?

Not really, there will always be new risks threats and vulnerabilities so making something completely invulnerable can be quite challenging. Things will constantly change and evolve. We can however, put in as much effort to coverour behinds as the others who are trying to break in even though we joke about it at times.

## Things I want to know more about
What are some common and uncommon cybersecurity threats that individuals and organizations face?

## References

[Many to many relationships](https://www.baeldung.com/hibernate-many-to-many)

[Security: a humorous overview](http://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf)