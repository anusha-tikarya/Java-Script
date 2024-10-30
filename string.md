
### What is a String?

A **string** is a sequence of characters used to represent text. In JavaScript, strings can include letters, numbers, symbols, and spaces.

### 1. Creating Strings

You can create strings in three ways:

#### Using Single Quotes

```javascript
let singleQuoteString = 'Hello, World!';
```

#### Using Double Quotes

```javascript
let doubleQuoteString = "Hello, World!";
```

#### Using Backticks (Template Literals)

```javascript
let templateString = `Hello, World!`;
```

**Template literals** are useful for multi-line strings and string interpolation (inserting variables).

### 2. String Properties and Methods

#### Length of a String

You can find out how many characters are in a string using the `length` property.

```javascript
let message = "Hello!";
console.log(message.length); // Outputs: 6
```

#### Common String Methods

Here are some frequently used string methods:

- **`toUpperCase()`**: Converts a string to uppercase.
  
  ```javascript
  let greeting = "hello";
  console.log(greeting.toUpperCase()); // Outputs: HELLO
  ```

- **`toLowerCase()`**: Converts a string to lowercase.
  
  ```javascript
  console.log(greeting.toLowerCase()); // Outputs: hello
  ```

- **`trim()`**: Removes whitespace from both ends of a string.
  
  ```javascript
  let spacedString = "   Hello!   ";
  console.log(spacedString.trim()); // Outputs: "Hello!"
  ```

- **`charAt(index)`**: Returns the character at a specified index.
  
  ```javascript
  console.log(greeting.charAt(1)); // Outputs: e
  ```

- **`indexOf(substring)`**: Returns the index of the first occurrence of a substring or `-1` if not found.
  
  ```javascript
  console.log(message.indexOf("o")); // Outputs: 4
  ```

- **`substring(startIndex, endIndex)`**: Extracts a portion of the string.
  
  ```javascript
  console.log(message.substring(0, 5)); // Outputs: Hello
  ```

### 3. String Concatenation

You can combine strings using the `+` operator or template literals.

#### Using the `+` Operator

```javascript
let firstName = "John";
let lastName = "Doe";
let fullName = firstName + " " + lastName;
console.log(fullName); // Outputs: John Doe
```

#### Using Template Literals

```javascript
let fullNameTemplate = `${firstName} ${lastName}`;
console.log(fullNameTemplate); // Outputs: John Doe
```

### 4. String Immutability

Strings in JavaScript are **immutable**, meaning once a string is created, it cannot be changed. Any operations that modify a string will create a new string instead.

```javascript
let originalString = "Hello";
let modifiedString = originalString.toUpperCase();
console.log(originalString); // Outputs: Hello (original remains unchanged)
console.log(modifiedString);  // Outputs: HELLO (new string)
```

### 5. Advanced String Manipulation

#### Split Method

You can split a string into an array of substrings using `split()`.

```javascript
let sentence = "Hello, how are you?";
let words = sentence.split(" ");
console.log(words); // Outputs: ["Hello,", "how", "are", "you?"]
```

#### Join Method

You can join elements of an array into a string using `join()`.

```javascript
let newSentence = words.join(" ");
console.log(newSentence); // Outputs: "Hello, how are you?"
```

### 6. Regular Expressions

Regular expressions (regex) are patterns used to match character combinations in strings. They can be used for searching, replacing, or validating strings.

#### Example: Using Regex to Test a String

```javascript
let regex = /hello/i; // 'i' makes it case-insensitive
let testString = "Hello, World!";
console.log(regex.test(testString)); // Outputs: true
```

### Summary

1. **Creating Strings**: Use single quotes, double quotes, or backticks.
2. **String Methods**: Learn methods like `length`, `toUpperCase()`, `trim()`, etc.
3. **Concatenation**: Combine strings with `+` or template literals.
4. **Immutability**: Strings cannot be changed after creation.
5. **Advanced Manipulation**: Use `split()` and `join()` for array operations.
6. **Regular Expressions**: Use regex for complex string matching and validation.


