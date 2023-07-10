# Java - Read 01



## Java Basics

What does “strong typed” mean?

In Java, being "strongly typed" means that the language enforces rules about how different types of data can be used together. It checks that variables and expressions are used in a way that makes sense based on their types. This helps catch mistakes and ensures that operations are done correctly.

What are the primitive data types?

In Java, there are eight primitive data types, which are the most basic data types built into the language. They are:

* boolean: Represents the boolean values true and false.

* byte: Represents 8-bit integer values ranging from -128 to 127.

* short: Represents 16-bit integer values ranging from -32,768 to 32,767.

* int: Represents 32-bit integer values ranging from -2,147,483,648 to 2,147,483,647.

* long: Represents 64-bit integer values ranging from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.

* float: Represents single-precision 32-bit floating-point values.

* double: Represents double-precision 64-bit floating-point values.

* char: Represents a single character using Unicode encoding.

These primitive types are used to store simple values directly, rather than references to objects. Java also provides a set of non-primitive types called reference types, which are built on top of these primitive types.


## XKCD: Compiling

Explain to a non-technical friend the difference in how compilation works in Java and JavaScript.

Compiling takes the code and checks them for errors, then converts the code into machine readable code that the computer can understand. The compiler makes sure that the code follows the rules of Java like using th correct tax and data types.

If there are any errors the compiler with point them out and will need to be fixed before the code can be successfully compiled.

JavaScript on the otherhand is an interpreted langauge. The code doesn't need to be compiled and can run directly in the browers. The code ran read from an engine that reads the code line by line and executes them on the spot. If there any errors the they will be reported durring execution.

Does code complining mean that it works correctly?

It does not guarantee that the program works correctly. Compilation just makes sures that the code is written following the rules of the language and catches the syntax errors. The code may not be working as intended depending on logical errors or bugs. You then need to test and debug to produce the desired outcome.

## Reading Java Documentation

How many keywords does Java have?

From this page it seems to have 51 key words

| Keyword | What It Does |
|---------|--------------|
| abstract | Indicates that the details of a class, a method, or an interface are given elsewhere in the code. |
| assert | Tests the truth of a condition that the programmer believes is true. |
| boolean | Indicates that a value is either true or false. |
| break | Jumps out of a loop or switch. |
| byte | Indicates that a value is an 8-bit whole number. |
| case | Introduces one of several possible paths of execution in a switch statement. |
| catch | Introduces statements that are executed when something interrupts the flow of execution in a try clause. |
| char | Indicates that a value is a character stored in 16 bits of memory. |
| class | Introduces a class - a blueprint for an object. |
| const | Reserved keyword in Java but not used. |
| continue | Forces the abrupt end of the current loop iteration and begins another iteration. |
| default | Introduces a path of execution to take when no case is a match in a switch statement. |
| do | Causes the computer to repeat some statements over and over again. |
| double | Indicates that a value is a 64-bit number with decimal precision. |
| else | Introduces statements that are executed when the condition in an if statement isn't true. |
| enum | Creates a newly defined type - a group of values that a variable can have. |
| extends | Creates a subclass that reuses functionality from a previously defined class. |
| final | Indicates that a variable's value cannot be changed, a class cannot be extended, or a method cannot be overridden. |
| finally | Introduces the last will and testament of the statements in a try clause. |
| float | Indicates that a value is a 32-bit number with decimal precision. |
| for | Causes the computer to repeat some statements a certain number of times. |
| goto | Reserved keyword in Java but not used. |
| if | Tests to see whether a condition is true. |
| implements | Indicates that a class provides bodies for methods declared in an interface. |
| import | Enables the programmer to use abbreviated names of classes defined in a package. |
| instanceof | Tests whether an object is an instance of a certain class. |
| int | Indicates that a value is a 32-bit whole number. |
| interface | Introduces an interface - a collection of method signatures. |
| long | Indicates that a value is a 64-bit whole number. |
| native | Enables the use of code written in a language other than Java. |
| new | Creates an object from a class. |
| package | Groups related classes and interfaces together. |
| private | Indicates that a variable or method can only be accessed within the same class. |
| protected | Indicates that a variable or method can be accessed within the same package or by subclasses. |
| public | Indicates that a variable, class, or method can be accessed from any other Java code. |
| return | Ends the execution of a method and returns a value. |
| short | Indicates that a value is a 16-bit whole number. |
| static | Indicates that a variable or method belongs to the class itself rather than instances of the class. |
| strictfp | Ensures strict floating-point behavior for intermediate calculations. |
| super | Refers to the superclass or parent class. |
| switch | Selects one of many possible cases for execution based on a given value. |
| synchronized | Prevents multiple threads from accessing the same code simultaneously. |
| this | Refers to the current object or instance of a class. |
| throw | Throws an exception or error to indicate an exceptional situation. |
| throws | Specifies the exceptions that a method may throw. |
| transient | Indicates that a variable does not need to be serialized when an object is serialized. |
| try | Introduces a block of code that is checked for exceptions. |
| void | Indicates that a method does not return a value. |
| volatile | Specifies that a variable may be modified asynchronously by multiple threads. |
| while | Repeats a block of code while a condition is true. |
| _ (underscore) | Reserved keyword in Java, currently not used. |

How do you print words to the console in Java?

``` java

public class Main {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}

```

## Things I want to know more about

TBD

### References

[Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

[Reddit thread on compiling](https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)

[XKCD: Compiling](https://xkcd.com/303/)

[Reading Java Documentation](https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/)