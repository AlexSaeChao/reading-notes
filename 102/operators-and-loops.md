# Operators and Loops

The loop header contains three parts: initialization, condition, and iteration. Initialization sets the loop variable to an initial value, the condition checks if the loop variable meets a certain condition, and iteration updates the loop variable after each iteration. When the condition is false, the loop stops, and control goes to the next statement after the loop.

While loop can potentially execute infinitely if the condition is never false, or if there is no exit condition specified inside the loop. To avoid infinite loops, we need to ensure the condition will eventually become false or that we include an exit condition.

### Questions From reading 08

* What is an expression in JavaScript?

**An expression in JavaScript is any code that gives a value. It can be a variable, a function call, an operator, or a mix of these. For instance, `4 + 3` is an expression that returns the value `7`.**

* Why would we use a loop in our code?

**We use loops in our code when we need to repeat instructions several times. This can make our code more efficient and avoid writing repetitive code. Loops are helpful when processing a large amount of data or when a task needs to be performed multiple times with or without input from user.**

* When does a for loop stop executing?

**A for loop stops when the condition specified in the loop header is false.**

* How many times will a while loop execute?

**A while loop will keep executing as long as the condition specified in the loop header is true.**