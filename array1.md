

### JavaScript Basics

- **Array**: A data structure that can store multiple values, both homogeneous (same type) and heterogeneous (different types).

### Storing a Value

To store the value `75` in JavaScript:
```javascript
let value = 75; // Using a variable
```

### JavaScript Type System

- **Is JavaScript Strictly Typed?**: No, JavaScript is loosely typed, meaning variables can hold any data type and can change types.

### Console Logging

To display a variable in the console:
```javascript
console.log(marks); // Replace 'marks' with your variable name
```

### Concept of Arrays

- Arrays are useful for storing multiple values, such as marks for multiple students:
```javascript
let marks = [75, 85, 90]; // Example array for three students
```

### Overcoming Limitations

- Arrays help overcome the limitation of single variable storage when handling bulk data.

### Dimensions of Arrays

- **1D Array**: A single list of values.
  ```javascript
  let oneDArray = [1, 2, 3];
  ```

- **2D Array**: An array of arrays (like a matrix).
  ```javascript
  let twoDArray = [[1, 2], [3, 4]];
  ```

- **3D Array**: An array of 2D arrays.
  ```javascript
  let threeDArray = [[[1]], [[2]]];
  ```

### Dimensions Explanation

- **D (Dimension)**: Refers to the number of indices needed to access an element. For example:
  - 1D: One index
  - 2D: Two indices
  - 3D: Three indices

### Minimum Elements in an Array

- Minimum elements in an array = 1 (an array can hold at least one item).


### What is an Object in JavaScript?

- **Object**: A collection of key-value pairs where keys are strings (or Symbols) and values can be any data type, including other objects, arrays, functions, etc.

Example of an object:
```javascript
let employee = {
    name: "John Doe",
    salary: 50000,
    location: "Pune"
};
```

### Salary of All Capgemini Employees in Pune

To represent the salary of all Capgemini employees located in Pune, you can use an array of objects, where each object represents an employee. This is often necessary when you have multiple employees.

Example:
```javascript
let employeesInPune = [
    { name: "Alice", salary: 60000, location: "Pune" },
    { name: "Bob", salary: 55000, location: "Pune" },
    { name: "Charlie", salary: 70000, location: "Pune" }
];
```
## Dimension: Refers to the number of indices required to access an element in an array. Each dimension adds a level of complexity to how you organize and access data.

## Index: The position of an element in an array. In JavaScript, array indices start at 0.


### Number of Dimensions Needed

- **1D Array**: If you only need to store the salaries of all employees in Pune, a simple 1D array of numbers would suffice:
    ```javascript
    let salaries = [60000, 55000, 70000];
    ```

- **2D Array**: If you need to store more complex data (e.g., salaries along with names and locations), a 2D array (array of objects) is ideal:
    ```javascript
    let employees = [
        ["Alice", 60000, "Pune"],
        ["Bob", 55000, "Pune"],
        ["Charlie", 70000, "Pune"]
    ];
    ```
  However, using an array of objects is more readable and manageable:
    ```javascript
    let employeesInPune = [
        { name: "Alice", salary: 60000 },
        { name: "Bob", salary: 55000 },
        { name: "Charlie", salary: 70000 }
    ];
    ```

### Why Use Objects?

- Objects provide better organization and readability, especially when dealing with multiple attributes (like name, salary, and location). They allow you to group related data together, making your code easier to understand and maintain.


### Array Basics

1. **Array Initialization**:
   - **Using Array Literal**:
     ```javascript
     let marks = [70, 80, 85];
     ```
   - **Using Array Constructor**:
     ```javascript
     let marks = new Array(70, 80, 85);
     ```

2. **Indexing**: 
   - Arrays are zero-indexed, meaning the first element is accessed with index `0`.
     ```javascript
     console.log(marks[0]); // Outputs: 70
     ```

3. **Slicing**:
   - Use the `slice()` method to extract a portion of an array:
     ```javascript
     let slicedMarks = marks.slice(1, 3); // Outputs: [80, 85]
     ```

4. **Dynamic Sizing**:
   - Arrays in JavaScript are not fixed in size; they can grow dynamically.
     ```javascript
     marks.push(60); // Adds 60 to the end of the array
     console.log(marks); // Outputs: [70, 80, 85, 60]
     ```

5. **Pushing Elements**:
   - You can add new elements to an array using the `push()` method:
     ```javascript
     let marks = []; // Start with an empty array
     marks.push(10); // Adds 10
     marks.push(20); // Adds 20
     marks.push(40); // Adds 40
     console.log(marks); // Outputs: [10, 20, 40]
     ```

6. **Creating an Array with Fixed Size**:
   - You can create an array of a specific size but it will be empty initially:
     ```javascript
     let marks = new Array(3); // Creates an array with 3 empty slots
     marks[0] = 60; // Fill the first slot
     marks[1] = 70; // Fill the second slot
     marks[2] = 80; // Fill the third slot
     console.log(marks); // Outputs: [60, 70, 80]
     ```

### Summary

- **Array Creation**: Use either array literals `[]` or the `new Array()` constructor.
- **Dynamic Resizing**: You can modify the size of arrays by adding or removing elements.
- **Slicing**: Use `slice()` to get a part of the array.
- **Indexing**: Access elements using zero-based indexing.


### 1. Using Array Literals

#### Create and Initialize
```javascript
let twoDArray = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
```

#### Display Elements
```javascript
console.log(twoDArray); // Outputs the entire 2D array
console.log(twoDArray[0][1]); // Outputs: 2 (first row, second column)
```

### 2. Using the `new Array()` Constructor

#### Create and Initialize
```javascript
let twoDArray = new Array(3); // Create an array with 3 rows
for (let i = 0; i < twoDArray.length; i++) {
    twoDArray[i] = new Array(3); // Create 3 columns for each row
}

// Initialize values
twoDArray[0][0] = 1;
twoDArray[0][1] = 2;
twoDArray[0][2] = 3;
twoDArray[1][0] = 4;
twoDArray[1][1] = 5;
twoDArray[1][2] = 6;
twoDArray[2][0] = 7;
twoDArray[2][1] = 8;
twoDArray[2][2] = 9;
```

#### Display Elements
```javascript
console.log(twoDArray); // Outputs the entire 2D array
console.log(twoDArray[1][2]); // Outputs: 6 (second row, third column)
```

### 3. Using Nested Loops for Initialization

#### Create and Initialize
```javascript
let rows = 3;
let cols = 3;
let twoDArray = new Array(rows);

for (let i = 0; i < rows; i++) {
    twoDArray[i] = new Array(cols);
    for (let j = 0; j < cols; j++) {
        twoDArray[i][j] = i * cols + j + 1; // Fill with incremental values
    }
}
```

#### Display Elements
```javascript
for (let i = 0; i < twoDArray.length; i++) {
    console.log(twoDArray[i]); // Outputs each row of the 2D array
}
```

### Summary

- **2D Array Definition**: You can use array literals or the `new Array()` constructor.
- **Initialization**: Use nested loops for dynamic initialization.
- **Displaying Elements**: Use `console.log()` for displaying entire arrays or specific elements by indexing.


### 3. `pop()`
- **What it does**: Removes the last element from an array and returns that element.
- **Example**:
  ```javascript
  let fruits = ['apple', 'banana', 'cherry'];
  let lastFruit = fruits.pop(); // Removes 'cherry'
  console.log(fruits); // Outputs: ['apple', 'banana']
  console.log(lastFruit); // Outputs: 'cherry'
  ```

### 4. `shift()`
- **What it does**: Removes the first element from an array and returns that element.
- **Example**:
  ```javascript
  let fruits = ['apple', 'banana', 'cherry'];
  let firstFruit = fruits.shift(); // Removes 'apple'
  console.log(fruits); // Outputs: ['banana', 'cherry']
  console.log(firstFruit); // Outputs: 'apple'
  ```

### 5. `indexOf()`
- **What it does**: Returns the index of the first occurrence of a specified element in the array. If the element is not found, it returns `-1`.
- **Example**:
  ```javascript
  let fruits = ['apple', 'banana', 'cherry'];
  let index = fruits.indexOf('banana'); // Outputs: 1
  console.log(index);
  ```

### 6. `includes()`
- **What it does**: Checks if an array contains a specified element. Returns `true` if found, otherwise `false`.
- **Example**:
  ```javascript
  let fruits = ['apple', 'banana', 'cherry'];
  let hasBanana = fruits.includes('banana'); // Outputs: true
  console.log(hasBanana);
  ```

### 7. `concat()`
- **What it does**: Merges two or more arrays into a new array.
- **What it does**: The `concat()` method is used to merge two or more arrays into a new array. It does not modify the existing arrays; instead, it creates and returns a new array containing the combined elements.

### Example

Here’s how to use `concat()`:

```javascript
let fruits1 = ['apple', 'banana'];
let fruits2 = ['cherry', 'date'];

// Using concat to merge arrays
let allFruits = fruits1.concat(fruits2);

console.log(allFruits); // Outputs: ['apple', 'banana', 'cherry', 'date']
```

### Additional Usage

You can also concatenate multiple arrays or even individual elements:

```javascript
let moreFruits = ['fig', 'grape'];

// Concatenating multiple arrays and elements
let combinedFruits = fruits1.concat(fruits2, moreFruits, 'kiwi');

console.log(combinedFruits); // Outputs: ['apple', 'banana', 'cherry', 'date', 'fig', 'grape', 'kiwi']
```

### Summary

- **Non-destructive**: `concat()` does not change the original arrays.
- **Returns a new array**: The result is a new array that includes all the concatenated elements.
- **Flexibility**: You can concatenate multiple arrays and additional elements at once.

This makes `concat()` a useful method for combining arrays in a clean and straightforward way! 


### 8. `sort()`
- **What it does**: Sorts the elements of an array in place and returns the sorted array. By default, it sorts elements as strings, which may lead to unexpected results with numbers.
- **Example**:
```javascript
let arr1 = [4, 2, 5, 3, 1];
console.log(arr1); // Outputs: [4, 2, 5, 3, 1]

arr1.sort();
console.log(arr1); // Outputs: [1, 2, 3, 4, 5] (sorted as strings)
```

**Note**: To sort numbers correctly, you can provide a compare function:
```javascript
arr1.sort((a, b) => a - b); // Sorts numerically
console.log(arr1); // Outputs: [1, 2, 3, 4, 5]
```

### 9. `reverse()`
- **What it does**: Reverses the order of the elements in an array in place and returns the reversed array.
- **Example**:
```javascript
arr1.reverse();
console.log(arr1); // Outputs: [5, 4, 3, 2, 1] (reversed order)
```

### Complete Example
Combining both methods:
```javascript
let arr1 = [4, 2, 5, 3, 1];
console.log(arr1); // Outputs: [4, 2, 5, 3, 1]

arr1.sort((a, b) => a - b); // Sort numerically
console.log(arr1); // Outputs: [1, 2, 3, 4, 5]

arr1.reverse();
console.log(arr1); // Outputs: [5, 4, 3, 2, 1]
```

### Summary
- **`sort()`**: Arranges array elements in order (string by default, numerical with a compare function).
- **`reverse()`**: Flips the order of the array elements.

let a = 10;
// if(a%2 == 0){
//     console.log("even");    
// }
// else{
//     console.log("odd");
// }
 
const result =  (a) => a%2 == 0 ? console.log("even"): console.log("odd");
result(a)
 
```javascipt 
let a = 10;
// if(a%2 == 0){
//     console.log("even");    
// }
// else{
//     console.log("odd");
// }
 
const result =  (a) => a%2 == 0 ? console.log("even"): console.log("odd");
result(a) 
```
### Original Code Explanation

1. **Variable Declaration**:
   ```javascript
   let a = 10; // Assigns the value 10 to the variable 'a'.
   ```

2. **If-Else Statement**:
   ```javascript
   if (a % 2 == 0) {
       console.log("even");    
   } else {
       console.log("odd");
   }
   ```
   - This checks if `a` is even by using the modulus operator (`%`). If `a` divided by `2` leaves no remainder (`0`), it's even; otherwise, it's odd.

### Refactored Using Arrow Function

3. **Arrow Function**:
   ```javascript
   const result = (a) => a % 2 == 0 ? console.log("even") : console.log("odd");
   result(a);
   ```
   - This is a concise way to define the same logic using an arrow function.
   - It takes `a` as a parameter and uses the ternary operator (`? :`) to determine if `a` is even or odd.
   - It calls the function `result(a)`, passing the value of `a`.

### Output
For `let a = 10`, both the original and the refactored code will output:
```
even
```

### Summary
- **Modulus Operator (`%`)**: Checks for evenness or oddness.
- **Arrow Function**: Provides a more concise syntax.
- **Ternary Operator**: A shorthand for `if-else` statements.

