# Arrow Functions

The are introduced in ES6 to produce a more concise syntax for writing functions in JavaScript.

They remove the need for the function keyword and have a shorter syntax.

__Before__
```
function add(a, b) {
  return a + b;
}
 
console.log(add(4, 12));
```
__After__
```
const add = (a, b) => a + b;
 
console.log(add(4, 12));
```

Arrow functions don't have their own `this` keyword. This means they cannot be used as object methods. However, they excel in scenarios such as __call back for array methods, event listeners, and situations where we want to simplify our code (function)__

https://js-docs-gamma.vercel.app/functions.html#arrow-functions