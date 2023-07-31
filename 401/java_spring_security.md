# Reading 16

## Spring Security overview

What does it mean to authenticate a user?

When you want to log in to a website or app, you have to prove that you are who you say you are. That process is called authentication. For example, you provide your username and password. The system checks if this information matches what it has on record. If they match, the system knows you are the real user, and you can access your account.

What does it mean to authorize a user?

Once the system knows who you are, it needs to decide what you are allowed to do. This is authorization. Think of it like having different levels of access in a building. Some people can go everywhere, some can only access certain rooms, and some can't enter at all. Similarly, the system checks your role or permissions to determine what parts of the website or app you can access and what actions you can perform.

What are the three possible outcomes of the AuthenticationManager’s authenticate() method?

Successful Authentication:

* If the provided credentials are valid, and the user is successfully identified, the authentication process is considered successful.

Failed Authentication:

* Now, if you made a mistake in your username or password, the system can't verify your identity. It will say something like, "Oops, the information you provided is incorrect. You can't access the account."

Unsupported Authentication Token:

* Sometimes, the AuthenticationManager may not support the provided authentication token type. In this case, the authenticate() method will return null or throw an AuthenticationException, indicating that the provided token is not supported.

## Things I want to know more about

## References

[Spring Security overview](https://spring.io/guides/topicals/spring-security-architecture/)

[Spring Auth cheat sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)
