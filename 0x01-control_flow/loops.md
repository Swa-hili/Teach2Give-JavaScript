# Loops

They enable execute block codes multiple times.

The loops in JavaScript are as follows:

-for loop
-for while loop
-do whie loop

## For loop

It is used when the number of blocked code to be executed is unknown.

The syntax is as follows:

```
for (initialization; condition; update) {

// code
}
```

-_Initialization_ is used to initialize the variable used in the loop.

-_Condition_ is used to evaluate the condition of the initial variable, if the condition returns true, the loop starts over again, if the condition returns false, the loop ends.

-_Update_ is used to update the initialization variable.

Example:

```
for (let i = 1; i <= 5; i++) {

console.log("Iteration:", i);
}
```


## While loop

This type of loop runs as long as a specified condition remains true.

```
while (condition) {

// code block to be executed if condition is true
}
```
Example:

```
let num = 1;

while (num <= 5) {

console.log("Number ", num);
num++;
}
```

## Do while loop

It executes the loop at least once, even if the condition is *false* from the start.

```
do {
/* code of block that will be
executed at least once even if
     condition is false */
} 

while (condition);
```

Example:

```
let x = 1;

do {
console.log("x ", x);
x++;
} while (x <= 5);
```

