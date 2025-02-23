# Destructuring
Destructuring is a convenient way to extract values from arrays or objects and assign them to variables in a single line.

# Destructuring Arrays

```
const numbers = [1, 2, 3];
const [first, second, third] = numbers;

console.log(first); // 1
console.log(second); // 2
console.log(third); // 3
```

We can also skip values when destructuring

```
const numbers = [1, 2, 3];
const [, , third] = numbers;

console.log(third); // 3
```

We can also use destructuring to swap variables

```
let a = 1, b = 2;

[a, b] = [b, a];

console.log(a); // 2
console.log(b); // 1
```
# Destructuring Objects

```
const person = {
  name: "Alice",
  age: 25,
};

const { name, age } = person;

console.log(name); // Alice
console.log(age); // 25
```

You can also rename variables when destructuring objects:

```
const person = {
  name: "Alice",
  age: 25,
};

const { name: firstName, age: yearsSinceBirth } = person;

console.log(firstName); // Alice
console.log(yearsSinceBirth); // 25
```

You can assign default value if the variable doesn't exist in an object:

```
const person = {
  name: "Alice",
  age: 25,
};

const {
  name: firstName,
  age: yearsSinceBirth,
  major = "Computer Science",
} = person;

console.log(firstName); // Alice
console.log(yearsSinceBirth); // 25
console.log(major); // Computer Science
```

We can use the rest operator to gather the remaining properties of an object during destructuring:

```
const person = {
  firstName: "Alice",
  lastName: "Doe",
  dateOfBirth: 2000,
  major: "Computer Science",
  profession: "Web Developer",
};

const { firstName, lastName, ...otherDetails } = person;
console.log(otherDetails);
// {
//   dateOfBirth: 2000,
//   major: 'Computer Science',
//   profession: 'Web Developer'
// }
```
