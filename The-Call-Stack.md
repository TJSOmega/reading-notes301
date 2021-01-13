[*From Free Code Camp freecodecamp.org*](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

**Last In, First Out (LIFO): it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.**

**Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.**

What causes a stack overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

In summary
The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

[*From Code burst io*](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)


**Types of error messages**

Reference errors
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

console.log(foo) // Uncaught ReferenceError: foo is not defined

This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).

Syntax errors
I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

Range errors
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

Type errors
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

