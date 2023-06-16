# In Memory Storage

In this section the reading talks about the call stack mechanism in JavaScript and some errors that might occur and what can be used to troubleshoot them.

## Understanding the JavaScript Call Stack

What is a ‘call’?

> The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution is done one at a time, from top to bottom. It means the call stack is synchronous.

How many 'calls' can happen at once?

One at a time.

What does LIFO mean?

Last in, first out. Kind of like popping and pushing in a stack.

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

``` javascript

function main() {
  function1();
}

function function1() {
  function2();
}

function function2() {
  function3();
}

function function3() {
}

main();

```

What causes a Stack Overflow?

> A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accommodate before throwing a stack error.

## JavaScript error messages

What is a ‘reference error’?

> This is as simple as when you try to use a variable that is not yet declared, you get this type of error.

``` javascript

console.log(foo) // Uncaught ReferenceError: foo is not defined

```

What is a 'syntax error'?

A syntax error is a type of error that occurs when the code violates the language's syntax rules and cannot be interpreted by the engine.

What is a 'range error'?

A range error occurs when a numeric value is outside the allowed value range. For example, when trying to access an index in an array that is outside its length.

What is a 'type error'?

A type error occurs when you try to manipulate data that is not supported or expected for a specific type. For example, trying to find the sum of numbers but including a string in the operation might cause a type error or unexpected behavior.

What is a 'breakpoint'?

A breakpoint is a designated point in the code where the execution will pause. It allows developers to inspect and debug the program's state, variables, and flow.

What does the word 'debugger' do in your code?

> The breakpoint can also be achieved by putting a debugger statement in your code on the line you want to break.

## Things I want to know more about

Nothing at this time.

## References

[The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

[JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
