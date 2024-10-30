
---

## **JavaScript Basics**

### 1. What is JavaScript?
- JavaScript is a high-level, interpreted programming language used to create interactive web pages.
- It can be run in web browsers, making it essential for web development.

### 2. Setting Up JavaScript
- You can run JavaScript in any web browser’s console (open it with F12).
- You can also create HTML files and include JavaScript in them using `<script>` tags.

### 3. Writing Your First JavaScript Code
```html
<!DOCTYPE html>
<html>
<head>
    <title>My First JavaScript</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <script>
        console.log("Hello, World!"); // Print to the console
    </script>
</body>
</html>
```

### 4. Basic Syntax
- **Comments**:
  - Single-line: `// This is a comment`
  - Multi-line: `/* This is a multi-line comment */`

### 5. Data Types
JavaScript has several data types:

#### a. Primitive Data Types
- **Number**: Represents both integers and floating-point numbers.
  ```javascript
  let age = 25; // Number
  let price = 19.99; // Floating point
  ```
- **String**: A sequence of characters.
  ```javascript
  let greeting = "Hello, World!";
  ```
- **Boolean**: Represents true or false values.
  ```javascript
  let isJavaScriptFun = true;
  ```
- **Undefined**: A variable that has been declared but not assigned a value.
  ```javascript
  let x; // x is undefined
  ```
- **Null**: Represents a deliberate non-value.
  ```javascript
  let y = null; // y is null
  ```

#### b. Reference Data Types
- **Object**: A collection of key-value pairs.
  ```javascript
  let person = {
      name: "Alice",
      age: 30
  };
  ```
- **Array**: A special type of object used to store ordered collections.
  ```javascript
  let colors = ["red", "green", "blue"];
  ```

### 6. Variables
You can declare variables using `var`, `let`, and `const`:

- **`var`**: Function-scoped or globally scoped (older way).
- **`let`**: Block-scoped (preferred for variable reassignment).
- **`const`**: Block-scoped, cannot be reassigned (for constants).

```javascript
var oldVariable = "I am old";
let newVariable = "I can change";
const constantVariable = "I don't change";
```

### 7. Control Structures
#### a. Conditional Statements
- **if statement**:
```javascript
if (age >= 18) {
    console.log("You are an adult.");
}
```
- **if-else statement**:
```javascript
if (age >= 18) {
    console.log("You are an adult.");
} else {
    console.log("You are a minor.");
}
```

#### b. Switch Statement
```javascript
let day = 3;
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    default:
        console.log("Invalid day");
}
```

### 8. Loops
#### a. For Loop
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

#### b. While Loop
```javascript
let count = 0;
while (count < 5) {
    console.log(count);
    count++;
}
```

### 9. Functions
#### a. Function Declaration
```javascript
function add(a, b) {
    return a + b;
}
```

#### b. Function Expression
```javascript
const subtract = function(a, b) {
    return a - b;
};
```

#### c. Arrow Function
```javascript
const multiply = (a, b) => a * b;
```

### 10. Arrays
- **Declaring and Initializing**:
```javascript
let fruits = ["apple", "banana", "cherry"];
```
- **Accessing Elements**:
```javascript
console.log(fruits[0]); // Outputs: apple
```
- **Common Array Methods**:
  - `push()`: Adds an element to the end.
  - `pop()`: Removes the last element.
  - `shift()`: Removes the first element.
  - `unshift()`: Adds an element to the beginning.
  - `slice()`: Extracts a portion of an array.
  - `splice()`: Adds/removes elements at specific indices.

### 11. Objects
- **Creating an Object**:
```javascript
let car = {
    brand: "Toyota",
    model: "Corolla",
    year: 2020
};
```
- **Accessing Properties**:
```javascript
console.log(car.brand); // Outputs: Toyota
```
- **Adding/Updating Properties**:
```javascript
car.color = "red"; // Add a new property
car.year = 2021; // Update existing property
```

### 12. Event Handling
JavaScript can respond to user events, like clicks or key presses.

```html
<button id="myButton">Click me!</button>
<script>
    document.getElementById("myButton").addEventListener("click", function() {
        alert("Button clicked!");
    });
</script>
```

### 13. Error Handling
- **Try-Catch Block**:
```javascript
try {
    let result = riskyOperation();
} catch (error) {
    console.log("Error occurred:", error);
}
```

### 14. Conclusion
- JavaScript is versatile and essential for web development.
- Practice by building small projects and experimenting with different features.

### Practice Tips
- Write small scripts to practice syntax and control structures.
- Explore JavaScript challenges on platforms like LeetCode or freeCodeCamp.

---

