# Reading 06

## Java OO Tutorial

What is the difference between an Object and a Class in Java?


Explain to a non-technical friend the concept of inheritance in Java.

Inheritance, Lets say you have a prototype blue print of a boat; base model, some thing that can float. You know that a boat can skim across water, hold passengers. Those are what properties of a boat class. From that bluw print you can make other kinds of boat as in speed boats, transport boats, amphibious; Adding on other properities of those boats. We can start making Objects of those boats with the blue print of the Boat class.

## Java Static Keyword

Static methods are also called what? Why?

They are also called class methods because they belong to a class instead of being an individual instance or onjects of the class. They can be accessed using the class name directly.

How can you access a variable of a class without instantiating an object from that class?

With dot notation you can access a variable of a class. For example, let's say we have a class called "MyClass" with a static variable called "myVariable." We can access this variable without creating an object of the class like this: `MyClass.myVariable`.

## Java Singleton Class

What is a Design Pattern? Describe one or two with analogies from your previous work experience.

It seems like a guarding a building with one way in and out. every who needs access may but there is only one door on this building.

> Create a `private` constructor of the class to restrict object creation outside of the class.
> Create a `private` attribute of the class type that refers to the single object.
> Create a `public static` method that allows us to create and access the object we created. Inside the method, we will create a condition that restricts us from creating more than one object.

What is a Singleton?

In Java, Singleton is a design pattern that ensures that a class can only have one object.

## Things I want to know more about

TBD

## References

[Java OO Tutorial (review Object and Class, read the rest)](https://docs.oracle.com/javase/tutorial/java/concepts/)

[Java Static Keyword](https://www.programiz.com/java-programming/static-keyword)

[Java Singleton Class](https://www.programiz.com/java-programming/singleton)