# Operators

Operators in JavaScript are symbols that perform operations on values (operands).

They are used for calculations, comparisons, and logical operations.

Operators in JavaScript are classified into the following categories:

- Arithmetic operators: perform basic mathematical operations.

- Assignment operators: assign values to variables.

- Comparison operators: compare values.

- Logical operators: used for boolean logic.

- Bitwise operators: perform operations at the binary level.

- Ternary operators


## Arithmetic Operators

These are used to perform mathematical operations.

__+ (addition)__

Adds two numbers:

```
let a = 10;
let b = 5;
console.log(a + b); // 15
It can also be used with strings to perform string concatenation:

let firstName = "John";
let lastName = "Doe";
console.log(firstName + lastName); // JohnDoe
```

__- (subtraction)__

Subtracts the right operand from the left:

```
let a = 10;
let b = 5;
console.log(a - b); // 5
```


__* (multiplication)__

Calculates the product of two numbers:

```
let a = 10;
let b = 5;
console.log(a * b); // 50
```


__/ (Division)__

```
let a = 10;
let b = 5;
console.log(a / b); // 2
```


__% (modulus/remainder)__

Returns the remainder of the division between the left and right operand.

```
let a = 10;
let b = 5;
console.log(a % b); // 0
```

__** (Exponentiation)__

```
let a = 10;
let b = 5;
console.log(a ** b); // 100000
```


### Increment Operator

Increases the variable's value by 1.

It can be used in two ways:

- Post-increment (a++): returns the original value and then increments it

- Pre-increment (--a): increments first then returns the updated value.

```
let x = 5;
console.log(x++); // 5 (returns first, then increments)
console.log(x); // 6

let y = 5;
console.log(++y); // 6 (increments first, then returns)
```


__Decrement Operator__

Decreases the variable's value by 1.

It can be used in two ways:

- Post-decrement (a--): returns the original value, then decrements.

- Pre-decrement (--a) – decrements first, then returns the updated value.

#### Assignment Operators

Used to assign values to variables

__= (Simple assignment operator)__

Used to assign a value to a variable

```
let x = 5;
```


__+= (Addition assignment operator)__
Used to add a value to a variable

let x = 5;
x += 3; // x = x + 3 → 8

__-= (Subtraction assignment operator)__
Subtracts a value from a variable

let x = 5;
x -= 2; // x = x - 2 → 3

__*= (Multiplication assignment operator)__
Multiples a variable

let x = 5;
x *= 2; // x = x * 2 → 10

__/= (Division Assignment Operator)__
Divides a variable

let x = 15;
x /= 3; // x = x / 3 → 5

##### Comparison Operator

They are used to compare values and they return true or false.

__== (Equality Operator)__
Returns true if the operand on the left is equal to the operand on the right and false otherwise.

let a = 10;
let b = 5;
console.log(a == b); // false
console.log(a == 10); // true
Note: The equality operator ignores the data type of the operands, it only compares the value:

console.log(10 == "10"); // true

__=== (Strict equality operator)__
Returns true if the operand on the left is equal to the operand on the right and false otherwise.

let a = 10;
let b = 5;
console.log(a === b); // false
console.log(a === 10); // true
Note: The strict equality operator checks the data type as well, not just the values:

console.log(10 === "10"); // false

__!= (Not equal/Inequality operator)__
Returns true if the value on the left is not equal to the value on the right and false otherwise.

It does not consider the data type of the operands.

let a = 10;
let b = 5;
console.log(a != b); // true
console.log(a != 10); // false

console.log(10 != "10"); // false

__!== (Strict not equal to/Strict inequality operator)__
Returns true if the value on the left is not equal to the value on the right and false otherwise.

It compares the data types of the operands.

let a = 10;
let b = 5;
console.log(a !== b); // true
console.log(a !== 10); // false

console.log(10 !== "10"); // true

__> (Greater than)__
Returns true if the operand on the left is greater than the operand on the right and false otherwise.

let a = 10;
let b = 5;
console.log(a > b); // true
console.log(b > a); // false

__< (Less than)__
Returns true if the operand on the left is less than the operand on the right and false otherwise.

let a = 10;
let b = 5;
console.log(a < b); // false
console.log(b < a); // true

__>= (Greater than or equal to)__
Returns true if the operand on the left is greater than or equal to the operand on the right.

let a = 10;
let b = 5;
console.log(a >= b); // true
console.log(b >= a); // false
console.log(10 >= 10); // true

__<= (Less than or equal to)__
Returns true if the operand on the left is less than or equal to the operand on the right.

let a = 10;
let b = 5;
console.log(a <= b); // false
console.log(b <= a); // true
console.log(10 <= 10); // true


###### Logical Operators

Used for boolean logic.

__Logical AND Operator (&&)__

The AND operator returns true only if both operands are true; otherwise, it returns false.

console.log(true && true); // true
console.log(true && false); // false

__Logical OR Operator (||)__
The OR operator returns true if at least one of the operands is true; otherwise it returns false.

console.log(true || true); // true
console.log(true || false); // true
console.log(false || false); // false

__Logical NOT operator (!)__
Used to negate boolean value of an expression, it returns true if the expression is false and returns false if the expression is true.

console.log(!true); // false
console.log(!false); // true