# Reading 02

The reading provides information on Java imports, built-in packages, different types of loops in Java, and Java arrays.

## Java Imports

Use an analogy to explain Built-In packages. Give examples.

Built in packages are kind of like a self stored tooling. Similar to a swiss army knife. Depending on what you want to create (writing code) you can pull out the desired tool(import package in the head of the file). For example if you wanted to use an array list you would import the java.util.Arraylist. This is because ArrayList class belongs to the java.util package.

Explain the steps for creating a new package in IntelliJ.

1. Right-click the src folder
2. select `new` and the `package`
3. name the package according to the directories nested in for example, `first` directory has a folder called `project`. The package would be called `first.project`. and would be imported by `import first.project`.

## Different types of loops in Java

Which loop types use a loop counter?

The Loop that uses a loop count is a for loop. Taking in a starting point, a boolean expresstion, and what to step up or down by. With all 3 parts they make a counter for a loop to use.

Explain the difference between While and Do-While loops.

The main difference betwen While and Do-While loops is that the expression gets evaluated in the beginning before the first iteration of the loop for While Loops. For Do-While loops the expression gets evaluated after the first iteration of the loop.

## Java Arrays

Describe 3 built-in methods for Arrays.

* `Array.toString()` method used for converting the array of ints returns a string enclosed in square brackets with each element seperated by a comma and a space.
* `Array.sort()` method is used for sorting elements in ascending order
* `Array.copyOf()` method is used to copy another array with a specified length modifer. used to resize or partially copy the targeted array.

How is the size of an array determined in Java?

The size of an array is determined at it's creation. It is fixed and can not be changed. You can set the size of an array when it  is created  by declaring a typeof, var name, assigning it a new int[] and size within the square bracket `int[] numbers = new int[5];`

## Things I want to learn more about

What are somethings you can do with a user defined package? I'm guessing you can create your own methods but not sure if it's a require package if you just nested the java file into just 1 directory. Besides the name needing to be unique what other reasons do they have to be named uniquely?

## References

[Java Import & Package - Programiz](https://www.programiz.com/java-programming/packages-import)

[Different types of loops in Java](https://www.baeldung.com/java-loops)

[Java Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)