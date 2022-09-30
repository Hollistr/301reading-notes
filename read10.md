# Class 301 Reading10

## Understanding the JavaScript Call Stack

1. What is a ‘call’?
    - A single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

2. How many ‘calls’ can happen at once?
    - One call at a time.

3. What does LIFO mean?
    - Last In, First Out

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
    - function firstFunction(){
        throw new Error('Stack Trace Error');
        }

        function secondFunction(){
        firstFunction();
        }

        function thirdFunction(){
        secondFunction();
        }

        thirdFunction();

5. What causes a Stack Overflow?
    - A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.

# JavaScript error messages

1. What is a ‘reference error’?
    - This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

console.log(foo) // Uncaught ReferenceError: foo is not defined


2. What is a ‘syntax error’?
    - Occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1

3. What is a ‘range error’?
    - Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length

4. What is a ‘type error’?
    -  the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

var foo = {}
foo.bar // undefined
foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined

5. What is a breakpoint?
    - Breakpoint is a place in your code, where you want the execution to stop to allow you to examine the program data and/or state.

6. What does the word ‘debugger’ do in your code?
    - The breakpoint can be achieved.

## Things I Want To Know More About

- More react, react, react!!!!

## Sources

- https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4

- https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
