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


2. ## Primitive types (2)
they are data types in javascript that are imutable(cannot be changed). they are also know us inbuilt data types.
eg: numbers, strings, boolean, null, undefined, symbol.
### Numbers
are data types that can hold  numeric values, both integers and floating-point numbers.
Strings are data types that represent a sequence of characters that are sorrounded by singel or double coats.
### Booleans
are data types that can accept only two values. ie true and false.
### Null
is a data type that can hold one possible value ie null or it is a declared binding or variable with the absence of a value.
### Undefined
is a variable declared without an assigned value.
### Symbols
are used to create unique identifiers for object properties. it is used to create objects that will always be unique. (ES2015).
### BigInts 
are used to store integers that too large to store us numbers. (ES2020).


02/05/2024
1. = means assignment operator.
2. Pure functions these are function that donot affect anything outside their scope.
