# reading 03

## Primitives vs. Objects

Explain the difference between an “int” and an “Integer” in Java.

"Int" is a primitive type in Java it has a fixed size of 32 bits nad direct stores the numerical value. It can not be null, but will have a default value of 0 if not assigned. unboxed

"Integer" is a wrappere class that serves as an Object representation of the "int" primittve. You can assign null to it at default if nothing is assigned. Autoboxed, assigns an int value without explicitly calling the constructor.

What is the default value for ints? Integers?

Ints: Default value 0
Integer: Default value null

What is autoboxing? Unboxing?

Int: Unboxing extract the numerical value from an "Integer" object and assign it to an "int" variable automatically.
Integer: Auttoboxing assign an "int" value to an "Integer" object directly without explicitly calling the constructor.

## Exceptions in Java (read the first three sections on the left: What is an Exception, The Catch or Specify Requirement, Catching and Handling Exceptions)

List the three basic categories of exceptions.

Checked: Checked exceptions checked by the compiler at compile time.
Unchecked: Exceptions don't need to be declared or cacught explictly.
Errors: Happen when something happens due to  an unrecoverable problem outside the control of the application, don't need to be caught or held.

What type of statement can you use to handle an exception?

Try Catch Statement, can use finally as well.

## Using Scanner to read in a file in Java

Describe a situation where you think it would be useful to have a program that scans text.

If you had a program that has some file processing or takes in user input. For the file processing, the application my be working witht text based data such as log files or config files.

What is input from a Scanner broken down into?

Input from a scanner is broken down into tokens. Tokens are units of text that separated by delimiters, like whitespace and punctuation marks. Scanner class provides methods to read tokens of different types like strings, ints, and floats.

## Things I want to know more about

Can I perform operations on primitive types and object types interchangeably?
Are there any performance differences between using primitives and objects?
How do I use the Scanner class to read user input from the console?

## References

[Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

[Exceptions in Java](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

[Using Scanner to read in a file in Java](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)
