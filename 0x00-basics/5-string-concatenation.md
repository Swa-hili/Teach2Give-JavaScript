# String Concatenation


String concatenation is the process of joining two or more strings together.

JavaScript provides multiple ways to concatenate strings.

## Using the + Operator

You can use the + operator to join strings together.

```
let firstName = "John";
let lastName = "Doe";
let fullName = firstName + lastName;
console.log("My full name is " + fullName);
```


### Using the += operator to append to an existing string
The += operator allows adding a string to an existing string.

```
let message = "Hello ";
message += "Dennis.";
console.log(message);
```


#### Using Template Literals

Template literals (introduced in ES6) use backticks (`) and '${}' placeholders for variables.

```
let firstName = "John";
let lastName = "Doe";
console.log(`My name is ${firstName} ${lastName}`);
```