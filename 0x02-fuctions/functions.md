# Functions

A function is a block of code that performs a specific task.

They help in writing modular, maintainable and reusable code.

In JavaScript, functions are *first-class citizens*; this means that they can be assigned to variables, passed as arguments, returned from other functions, stored in data structures and even created dynamically.

The basic syntax for declaring a function in JavaScript is as follows:

```
function functionName() {

// function body
}
function printHello() {

console.log("Hello, world");
}
```

To use a function, you must call/invoke the function as shown:

```
function printHello() {

console.log("Hello, world");
}

// calling/invoking a function
printHello();
```


# Parameters vs Arguments

A __parameter__ is a variable declared in a function definition and acts as a placeholder for the value that will be passed to the function when the function is being called.

An __argument__ is the actual value passed to a function when it is called, it provides the data that the function or the method will operate on.

function greet(name) { // name is a parameter

```
console.log(`Hello ${name}`);
}

greet("John Doe"); // John Doe is an argument
```


# Function Return Values

A function can return a value using the return keyword.

function add(number1, number2) {
  return number1 + number2;
}

let sum = add(35, 23);
console.log(sum);

## Categories of Functions

Functions can be categorized as follows:

- Functions that don't take parameter(s) and don't return a value

- Functions that don't take parameter(s) but return a value

- Functions that take parameter(s) but don't return a value.

- Functions that take parameter(s) and return a value.

__Functions that don't take parameter(s) and don't return a value__

These functions don't take any parameter(s) and don't return any values.

```
function add() {
  let a = 55;
  let b = 68;
  console.log(a + b);
}

add();
```

__Functions that don't take parameter(s) but return a value__

These functions don't take any parameter(s), but they return a value.

```
function add() {
  let a = 55;
  let b = 68;
  return a + b;
}

console.log(add());
```


__Functions that take parameter(s) but don't return a value__

These functions take parameter(s) but don't return a value.

```
function add(a, b) {

console.log(a + b);
}
add(5, 3);
```


__Functions that take parameter(s) and return a value__

These functions take in parameter(s) and return a value.

```
function add(a, b) {
  return a + b;
}
console.log(add(5, 3));
```


# Types of functions in JavaScript

JavaScript has the following types of functions:

- Function declaration

- Function expression/anonymous function

- Arrow functions

- Immediately Invoked Function Expression (IIFE)

- Callback functions

## Function declaration

```
function add(a, b) {
  console.log(a + b);
}

add(5, 2);
```


## Function expression/anonymous function

Involves saving a function to a variable.

```
let add = function (a, b) {
  console.log(a + b);
}

add(5, 2);
```

## Arrow functions

Arrow functions were introduced in ES6 and are used to simplify how we write functions.

```
let add = (a, b) => {
return a + b;
}

console.log(add(5, 2));
```

If an arrow function has only one line in the body, we can get rid of the curly braces

This means that instead of:

```
let add = (a, b) => {
  console.log(a + b);
}

add(5, 2);
We can write:

let add = (a, b) => console.log(a + b);
``` 

If an arrow function has only one line of code in the body and that line happens to be a return statement, we can get rid of the return keyword:

```
let add = (a, b) => a + b;

console.log(add(5, 2));
```

If an arrow function has only one parameter, we can get rid of the parenthesis:

```
let square = number => number * number;

console.log(square(8)); // 64
```


## Immediately Invoked Function Expressions (IIFE)

These functions are executed immediately after being defined:

```
(function () {

console.log("Hello, World!");
})();
```

These functions can also take parameters:

```
(function (a, b) {
  
  let sum = a + b;
  
  let product = a + b;
  
  console.log(`The sum of ${a} and ${b} is ${sum}`);
  console.log(`The product of ${a} and ${b} is ${product}`);
})(5, 6);
```


## Callback functions

Refer to functions passed as arguments to other functions.

```
function greet(name, callback) {
  
  console.log(`Hello ${name}`);
  callback();
}

greet("Dennis", function () {
  
  console.log("Welcome back");
});
```