# learning-33-concepts-of-js

01/05/24
1. ## Call Stack (1)
-  When a function is called, a new entry representing that function call is added to the top of the call stack. Similarly, when a function returns, its entry is removed from the stack. This process of adding and removing function calls from the stack follows a Last-In-First-Out (LIFO) principle.
-  It ensures that functions are executed in the correct order and that the program behaves as expected. If the call stack becomes too large (due to too many nested function calls), it can lead to a stack overflow error.
- When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. 
In summary
The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

eg:
```
function firstFunction() {
    secondFunction();
}
function secondFunction() {
    thirdFunction();
}
function thirdFunction() {
    // Do something
}
firstFunction(); // Initial function call
```
