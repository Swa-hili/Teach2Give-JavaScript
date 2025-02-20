# Arrays

An array is a collection of elements stored at contiguous memory locations.

An array is a special variable, which can hold more than one value.

An array can hold many values under a single name, and you can access the values by referring to an index number.

# Creating an array

You can create an array in one of the following ways:

An array literal

The new Array() constructor.

## Using an array literal

const arrayName = [item1, item2, item3, ...];

Example:

```
const students = ["John", "Ken", "June", "Jack"];

You can also nest arrays within arrays (multidimensional arrays):

const arr = [1, 2, 3, [4, 5, 6, [90, 80]], [20, 30, 40]];
```

## Using the new Array() constructor

const arrayName = new Array(item1, item2, item3, ...)

Example:
```
const students = new Array("John", "Ken", "June", "Jack");
new Array() constructor can also be nested:

const arr = new Array(1, 2, new Array(5, 6, new Array(30, 40)));
```

Always use array literal to create an array.

# Accessing array elements

You access an array element by referring to the index number.

The first element has index 0, the second element index 1, e.t.c.

```
const students = ["John", "Ken", "June", "Jack"];
console.log(students[0]); //John

console.log(students[1]); //Ken

console.log(students[2]); //June
```


# Basic Array Methods

## 1. Length of an array

The length property returns the length (size) of an array.

The length of an array refers to the number of items in the array.

```
const students = ["John", "Ken", "June", "Jack"];
console.log(students.length); // 4
```

## 2. pop()

The pop method removes the last item of an array.

```
const students = ["John", "Ken", "June", "Jack"];
students.pop();

console.log(students); //[ 'John', 'Ken', 'June' ]
```

Note: the pop method returns the element that was removed

## 3 push()

The push method adds a new element at the end of the array.

```
const students = ["John", "Ken", "June", "Jack"];
students.push("Nancy");

console.log(students); // ['John', 'Ken', 'June', 'Jack', 'Nancy']
```

You can also add multiple elements using the push method:

```
const students = ["John", "Ken", "June", "Jack"];
students.push("Nancy", "Miriam", "Simon");
```

The push method returns the new length of the array.

## 4. shift()

The shift method removes the first element of an array.
```
const students = ["John", "Ken", "June", "Jack"];
students.shift();

console.log(students); // ['Ken', 'June', 'Jack']
```

The shift method returns the element that was removed.

## 5. unshift()

The unshift method adds an element to the start of an array.

```
const students = ["John", "Ken", "June", "Jack"];
students.unshift("Nancy");

console.log(students); // ['Nancy', 'John', 'Ken', 'June', 'Jack']
```

You can also add multiple elements using the unshift method:

```
const students = ["John", "Ken", "June", "Jack"];
students.unshift("Nancy", "Miriam", "Simon")
```

## 6. at()

The at method returns an element at the specified index

```
const students = ["John", "Ken", "June", "Jack"];
console.log(students.at(2)); // June
console.log(students.at(0)); // John
```

## 7. Join()

The join() method also joins all array elements into a string.

It behaves just like toString(), but in addition, you can specify the separator:

```
const students = ["John", "Ken", "June", "Jack"];
console.log(students.join("++")); // John++Ken++June++
```

## 8. Concat()

The concat() method creates a new array by merging (concatenating) existing arrays:

```
const arr1 = ["jack", "franklin", "june"];

const arr2 = ["andrew", "alex", "ken"];
console.log(arr1.concat(arr2));
// [ 'jack', 'franklin', 'june', 'andrew', 'alex', 'ken' ]
```

## 9. Flat()

The flat method converts a multidimensional array to a one-dimension array.

```
const students = [

  ["jack", "franklin"],
  
  ["june", "andrew"],
  
  ["alex", "ken"],
];

console.log(students.flat());
// ['jack', 'franklin', 'june', 'andrew', 'alex', 'ken']
```

## 10. IndexOf()

The indexOf() method is used to find the index of an element.

It returns -1 if the element is not found.

```
const students = ["John", "Ken", "June", "Jack"];
console.log(students.indexOf("June")); // 2
```

## 11. Includes()

Checks if an element exists in an array.

It returns true if it exists and false if it doesn't.

const students = ["John", "Ken", "June", "Jack"];
console.log(students.includes("Ken")); // true
console.log(students.includes("Elvis")); // false

## 12. Reverse()

Reverses the elements of an array.

const students = ["John", "Ken", "June", "Jack"];
console.log(students.reverse());