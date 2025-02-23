# Asynchronous JavaScript

Asynchronous JavaScript refers to the execution of JavaScript without blocking the main thread, allowing other operations to continue while waiting for other tasks to complete.

This is essential for tasks such as network requests, file reading, and timers which can take an unknown amount of time.

JavaScript is inherently single-threaded and synchronous. This means it processes one task at a time sequentially.


With asynchronous programming, JavaScript programs can start long-running tasks, and continue running other tasks in parallel.

In JavaScript, asynchronous programming is done using `Promises`.

__Example of what asynchronous JavaScript looks like:__

```
setTimeout(() => {
  console.log("Asynchronous JavaScript");
}, 2000);

console.log("Hello World");
console.log("Goodbye World");

// Output:
// Hello World
// Goodbye World
// Asynchronous JavaScript
```
