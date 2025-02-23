# Spread Operator
The spread operator (...) allows you to expand elements of an iterable (like arrays, objects, or strings) into individual elements.

# Use Case of the Spread Operator
## Expanding an Array
The spread operator takes the array elements and spreads them individually.

Example:

```
const numbers = [1, 2, 3];
console.log(...numbers); // 1 2 3

const names = ["John", "Doe"];
console.log(...names); // John Doe
```
## Copying Arrays
The spread operator can be used to copy array elements, which helps avoid mutate the original array.

For example, instead of;

```
const original = [1, 2, 3];
const copy = original;

copy.push(55);
```

We can copy an array as shown:

```
const original = [1, 2, 3];
const copy = [...original];
```

## Merging Arrays
We can use the`spread operator` to merge an array:

```
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const merged = [...arr1, ...arr2];

console.log(merged); // [1, 2, 3, 4, 5, 6]
```

## Adding elements from one array to another

```
const numbers = [2, 3, 4];
const newNumbers = [1, ...numbers, 5];

console.log(newNumbers); // [1, 2, 3, 4, 5]
```

## Copying objects

```
const person = { name: "John", age: 25 };
const copy = { ...person };

console.log(copy); // Output: { name: "John", age: 25 }
```

## Merging objects

```
const obj1 = { name: "John" };
const obj2 = { age: 25 };
const merged = { ...obj1, ...obj2 };

console.log(merged); //  { name: "John", age: 25 }
```

## Ovewriting Properties

```
const user = { name: "John", role: "User" };
const updatedUser = { ...user, role: "Admin" };

console.log(updatedUser); // { name: "John", role: "Admin" }
```
