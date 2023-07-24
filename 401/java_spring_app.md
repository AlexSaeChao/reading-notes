# Reading 11

## Spring App Basics

What role do the @Controller classes play in a Spring MVC application?

They act as handlers for requests and hold instructions on what to do with responses. Think of it like reactive specialized middlemen that deal with requests and responses when they come across their specific handler/controller.

Explain to a non-technical friend what a GET request is.

A Get request is like a drive through bank teller with the vacuum capsules to request your balance in your account in the 90's. You could talk to the tell via mic and sometimes be asked to fill out paperwork and send back via by the chute and capsule. This would be your request to the bank signifiying that your like to see your balance. After request recieved and ID verified, they will send a printout with the information. The request from the browser would be like you asking to see your balance. GET is specificly just a READ request. Finally, the response from the teller would be the response the server sends back if everything else matched.

What annotation should be placed on your Spring Boot application class?

> `@SpringBootApplication` is a convenience annotation that adds all of the following:
> * `@Configuration`: Tags the class as a source of bean definitions for the application context.
> * `@EnableAutoConfiguration`: Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings. For example, if spring-webmvc is on the classpath, this annotation flags the application as a web application and activates key behaviors, such as setting up a DispatcherServlet.
> * `@ComponentScan`: Tells Spring to look for other components, configurations, and services in the com/example package, letting it find the controllers.

## Spring MVC and Thymeleaf

What method allows for a variable defined in Java (in your Spring Controller) to be displayed in HTML with the help of Thymeleaf?

Model.addAttribute is used to display HTML with the help of Thymeleaf.

Explain the role of a @Controller class in a Spring MVC application.

The `@Controller` class serves as the entry point for handling incoming HTTP requests, processing the data, and directing the flow of information between the user and the application's backend.

What is a model attribute refered to in Thymeleaf?

A model attribute refers to the data that is passed from the Spring Controller to the Thymeleaf template for rendering.
When a controller method returns the name of a template, Spring will take care of populating the model attributes into the template, making them available for use within the HTML content.

## Things I want to know more about

What are the advantages of using Spring MVC and Thymeleaf over traditional server-side web frameworks?
Are there any best practices for organizing the code and structuring the project in a Spring MVC application?

## References

[Spring App Basics](https://spring.io/guides/gs/serving-web-content/)

[Spring MVC and Thymeleaf](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)
