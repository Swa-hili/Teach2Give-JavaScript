# Conditionals

They allow you to execute different blocks code based on specific conditions.

Conditional statements in JavaScript include:

- if statement

- if else statement

- if else ladder

- switch statement

## If statement

It is used to execute a block of code if a specified condition is true.

The syntax is as follows:

```
if (condition) {

// block of code to be executed if the condition is true
}
```

Example in code:

```
let age=30
if (age>20){
console.log("You are a youth")
}
```

## If else statement

Executes the code in the _if_ block when the condition is true, if the condition is false, the code inside the else block gets executed.

```
if (condition) {

// block of code to be executed if the condition is true
} 

else {

// block of code to be executed if the condition is false
}
```

Example in code:

```
let age = 15;
if (age > 19) {
console.log("You are an adult");
} 

else {
console.log("You are a child");
}
```

## If else ladder

Used when multiple conditions need to be checked sequentially.

It uses the following syntax:

```
if (condition1) {

// block of code to be executed if condition1 is true
} 

else if (condition2) {

// block of code to be executed if condition1 is false and condition2 is true
} 

else {
// block of code to be executed if both condition1 and condition2 are false
}
```

Example in code:

```
let marks = 85;
if (marks >= 90) {
console.log("Grade: A");
} 
else if (marks >= 80 && marks < 90) {
console.log("Grade: B");
} 
else if (marks >= 70 && marks < 80) {
console.log("Grade: C");
} 
else {
console.log("Grade: F");
}
```

## Switch Statement

Used when a variable has multiple possible values. It is cleaner than multiple if..else
if conditions.

The syntax is as follows:

```
switch (expression) {
case value1:
    // block of code to be executed if expression === value1
    break;
case value2:
    // block of code to be executed if expression === value2
    break;
default:
// block of code to be executed if expression doesn't match any case
}
```

Example in code:

```
let day = "Monday";
switch (day) {
  case "Monday":
    console.log("Start of the work week.");
    break;
  case "Friday":
    console.log("Weekend is near!");
    break;
  case "Sunday":
    console.log("It's a rest day.");
    break;
  default:
    console.log("It's a regular day.");
}
```


# Ternary Operator

It provides a concise way to write if-else statements in a single line.

The syntax is:

```
condition ? expression if condition is true : expression if condition is false
```

Example in code:

```
const age = 35;

age > 18 ? console.log("You are an adult") : console.log("You are a child");
```









