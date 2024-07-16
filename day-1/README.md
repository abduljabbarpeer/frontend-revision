# HTML/CSS

## HTML

### Tags, Elements, and Attributes

- **Tags**:
  ```html
  <h1>Title</h1>
  <p>Paragraph text here.</p>
  ```
- **Elements**:
  ```html
  <p>This is a paragraph.</p>
  ```
- **Attributes**:
  ```html
  <a href="https://example.com" target="_blank">Visit Example</a>
  ```

### Div, Span, and Classes

- **`<div>`**:
  ```html
  <div class="container">
    <p>Content inside a div.</p>
  </div>
  ```
- **`<span>`**:
  ```html
  <p>This is <span class="highlight">highlighted</span> text.</p>
  ```
- **Classes**:
  ```html
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  ```

### Hyperlinks and Media

- **Hyperlinks**:
  ```html
  <a href="https://example.com">Visit Example</a>
  ```
- **Images**:
  ```html
  <img src="image.jpg" alt="Description of image" />
  ```
- **Videos**:
  ```html
  <video src="video.mp4" controls></video>
  ```

### Tables

- **Basic Structure**:
  ```html
  <table>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </table>
  ```

### Forms and APIs

- **Forms**:
  ```html
  <form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" />
    <button type="submit">Submit</button>
  </form>
  ```

---

## CSS

### Syntax and Selectors

- **Syntax**:
  ```css
  selector {
    property: value;
  }
  ```
  Example:
  ```css
  p {
    color: blue;
  }
  ```
- **Selectors**:
  - **Element Selector**:
    ```css
    p {
      font-size: 16px;
    }
    ```
  - **Class Selector**:
    ```css
    .className {
      background-color: yellow;
    }
    ```
  - **ID Selector**:
    ```css
    #idName {
      text-align: center;
    }
    ```

### Box Model

- **Components**:
  ```css
  div {
    margin: 10px;
    border: 1px solid black;
    padding: 5px;
    width: 100px;
  }
  ```

### Properties like `justify-content` and `text-align`

- **`justify-content`**:
  ```css
  .container {
    display: flex;
    justify-content: center;
  }
  ```
- **`text-align`**:
  ```css
  p {
    text-align: center;
  }
  ```

### Layouts like Flexbox and Grid

- **Flexbox**:
  ```css
  .container {
    display: flex;
    justify-content: space-between;
  }
  ```
- **Grid**:
  ```css
  .container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
  ```

### Animations

- **Basic Animation**:

  ```css
  @keyframes example {
    from {
      background-color: red;
    }
    to {
      background-color: yellow;
    }
  }

  div {
    animation-name: example;
    animation-duration: 4s;
  }
  ```

## JavaScript Guide

### Constants & Variables

- **Constants**: Immutable values that cannot be reassigned.
  ```javascript
  const pi = 3.14;
  ```
- **Variables**: Mutable values that can be reassigned.
  ```javascript
  let age = 25;
  age = 26;
  var name = "John";
  name = "Doe";
  ```

### Data Types

- **Primitive Types**: Number, String, Boolean, Null, Undefined, Symbol.
  ```javascript
  let number = 42; // Number
  let text = "Hello"; // String
  let isTrue = true; // Boolean
  let empty = null; // Null
  let notDefined; // Undefined
  ```

### Conditional Statements

- **If-Else**: Execute code based on conditions.
  ```javascript
  let score = 85;
  if (score >= 90) {
    console.log("A");
  } else if (score >= 80) {
    console.log("B");
  } else {
    console.log("C");
  }
  ```

### Loops

- **For Loop**: Iterate over a block of code a number of times.
  ```javascript
  for (let i = 0; i < 5; i++) {
    console.log(i);
  }
  ```
- **While Loop**: Execute code as long as a condition is true.
  ```javascript
  let i = 0;
  while (i < 5) {
    console.log(i);
    i++;
  }
  ```

### Operators

- **Arithmetic Operators**: Perform mathematical operations.
  ```javascript
  let sum = 5 + 3; // 8
  let product = 4 * 2; // 8
  ```
- **Comparison Operators**: Compare values.
  ```javascript
  let isEqual = 5 == "5"; // true
  let isIdentical = 5 === "5"; // false
  ```

### Functions

- **Function Declaration**: Define a reusable block of code.
  ```javascript
  function greet(name) {
    return `Hello, ${name}!`;
  }
  console.log(greet("Alice"));
  ```
- **Arrow Function**: A shorter syntax for writing functions.
  ```javascript
  const greet = (name) => `Hello, ${name}!`;
  console.log(greet("Alice"));
  ```

### Arrays

- **Creating Arrays**: A collection of items.
  ```javascript
  let fruits = ["apple", "banana", "cherry"];
  ```
- **Array Methods**: Common operations on arrays.
  ```javascript
  fruits.push("date"); // Add to end
  fruits.pop(); // Remove from end
  console.log(fruits[1]); // Access item at index
  ```

### Strings

- **String Methods**: Manipulate and extract information from strings.
  ```javascript
  let message = "Hello, World!";
  console.log(message.length); // 13
  console.log(message.toUpperCase()); // "HELLO, WORLD!"
  console.log(message.substring(0, 5)); // "Hello"
  ```

### JSON

- **JSON**: JavaScript Object Notation, used for data exchange.
  ```javascript
  let jsonString = '{"name": "Alice", "age": 25}';
  let jsonObject = JSON.parse(jsonString);
  console.log(jsonObject.name); // "Alice"
  let newJsonString = JSON.stringify(jsonObject);
  ```

### DOM Manipulations

- **Selecting Elements**: Access elements in the HTML document.
  ```javascript
  let element = document.getElementById("myElement");
  let elements = document.getElementsByClassName("myClass");
  let queryElement = document.querySelector(".myClass");
  ```
- **Changing Content**: Modify the content of elements.
  ```javascript
  element.textContent = "New Content";
  element.innerHTML = "<strong>Bold Content</strong>";
  ```
- **Event Listeners**: Respond to user interactions.
  ```javascript
  element.addEventListener("click", () => {
    alert("Element clicked!");
  });
  ```
