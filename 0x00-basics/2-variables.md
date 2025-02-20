# VARIABLES

It is a labeled container that holds a piece of information.

 A value- It is the actual piece of information that is stored in a variable.It can be:
 - A number
 - Text
 - Or a function

A constant- It is a value that does not change.


## Declaring Variables in JavaScript

They can be declared in three ways:
1. var: It is old, avoid using it to pretend scope-related issues.
2. let: It used for variables that change.
3. const: Variables that do not change.


### Updating Variables

They can be updated using var and let.
```
let percentage = 20;
percentage= 60; // Now the value of "percentage" is updated to 80
var item = "Book";
item = "Pen";
const Continent = "Africa";
```


### Declaring Vs. Initializing Variables

__Declaring Variables__

This is where a variable is created but it has no value assigned to it. This tells JavaScript that the variable exists, but it does not have any value yet.
```
let kg; // Declared but not initialized
console.log(kg); // Output: undefined

After defining the variable;

let ; // Declared but not initialized
age = 50;
console.log(age); // Output: 50
```


__Initializing a Variable__

Assigning a variable an initial value during declaration.
```
let kg = 40; // Declared and initialized with a value
console.log(kg); // Output: 40
```

#### Rules for naming Variables
- Variable names can only start with a letter, an underscore or a dollar sign.
```
let color = "Blue";
let _percentage = 70;
let $cost = 85.50;
```

- Variables names cannot be JavaScript reserved keywords.
```
let let = "Rwanda"; // ❌ "let" is a reserved keyword
let function = 20; // ❌ "function" is a reserved keyword
```


- Variable names are case-sensitive

 JavaScript differentiates between uppercase and lowercase
```
let Color = Red;
let color = Red;
console.log(Color); // Red
console.log(color); // Red
```


- Use meaningful and descriptive names
```
let userName = "Sencier";
let totalPrice = 200;
let isLoggedIn = true;
```

- If a variable name is made up of multiple words, use the camel case convention.
```
let userName = "Sencier";
let totalPrice = 200;
let isLoggedIn = true;
```



















