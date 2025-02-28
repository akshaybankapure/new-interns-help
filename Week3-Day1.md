### **📅 Day 1: JavaScript Syntax, Variables & Operators (For Absolute Beginners)**  

### **Session 1: Introduction to JavaScript & Variables**  

#### **What is JavaScript?**  
JavaScript is a **programming language** used to make web pages interactive. It allows you to add animations, handle user input, and communicate with servers.

#### **How to Run JavaScript?**  
You can run JavaScript in:  
1. **Browser Console** (Press `F12` in Chrome → Go to `Console` tab → Type `console.log("Hello, JavaScript!")` and press Enter)  
2. **Inside an HTML File** (Create an HTML file and include JavaScript inside a `<script>` tag)
   ```html
   <html>
     <body>
       <h1>Hello JavaScript!</h1>
       <script>
         console.log("This is JavaScript running in the browser.");
       </script>
     </body>
   </html>
   ```
3. **External JavaScript File** (Recommended for large projects)  
   - Create a new file, e.g., `script.js`, and include it in your HTML file:  
   ```html
   <script src="script.js"></script>
   ```

#### **Declaring Variables**  
Variables are **containers** used to store data.  
JavaScript has three ways to declare variables:  
1. **`var`** (Old way, avoid using it)  
2. **`let`** (Use when the value **might** change)  
3. **`const`** (Use when the value **won’t change**)  

Example:
```js
let name = "Alice";  // Can be changed later
const age = 25;  // Cannot be changed later
var oldSyntax = "Avoid using var";  // Not recommended
```
💡 **Hint:** Always prefer `const` unless you **need** to change the value.

#### **Understanding Hoisting**  
- JavaScript **moves (hoists)** variables **declared with `var`** to the top of the script before execution, but **doesn’t initialize them**.  
- `let` and `const` **are hoisted but not initialized**, meaning you **cannot use them before declaration**.

Example:
```js
console.log(x); // Undefined (Hoisted but not initialized)
var x = 10;
```
Using `let`:
```js
console.log(y); // Error: Cannot access 'y' before initialization
let y = 10;
```

---

### **Session 2: Data Types & Operators**  

#### **Data Types in JavaScript**  
JavaScript has **7 primitive data types**:
1. **Number** – Example: `10`, `3.14`
2. **String** – Example: `"Hello"`, `'JavaScript'`
3. **Boolean** – Example: `true`, `false`
4. **Null** – Intentional empty value (`let x = null;`)
5. **Undefined** – Variable declared but not assigned a value (`let y;`)
6. **Symbol** – Used for unique values
7. **BigInt** – For very large numbers (`BigInt(9999999999999999)`)

Example:
```js
let number = 42;  // Number
let text = "Hello, World!";  // String
let isJavaScriptFun = true;  // Boolean
let emptyValue = null;  // Null
let notAssigned;  // Undefined
```

💡 **Hint:**  
- `typeof` checks the data type of a variable:  
  ```js
  console.log(typeof 42); // "number"
  console.log(typeof "Hello"); // "string"
  console.log(typeof true); // "boolean"
  console.log(typeof undefined); // "undefined"
  console.log(typeof null); // "object" (This is a known JavaScript bug)
  ```

---

### **Operators in JavaScript**  

#### **Arithmetic Operators**  
| Operator | Example | Meaning |
|----------|----------|---------|
| `+` | `5 + 3` → `8` | Addition |
| `-` | `5 - 2` → `3` | Subtraction |
| `*` | `4 * 3` → `12` | Multiplication |
| `/` | `10 / 2` → `5` | Division |
| `%` | `10 % 3` → `1` | Modulus (Remainder) |
| `**` | `2 ** 3` → `8` | Exponentiation (Power) |

Example:
```js
let sum = 5 + 3;  // 8
let remainder = 10 % 3;  // 1
let power = 2 ** 3;  // 8
```

#### **Comparison Operators**  
| Operator | Example | Meaning |
|----------|----------|---------|
| `==` | `5 == "5"` → `true` | Equality (ignores type) |
| `===` | `5 === "5"` → `false` | Strict Equality (checks type too) |
| `!=` | `10 != "10"` → `false` | Not equal |
| `!==` | `10 !== "10"` → `true` | Strict Not equal |
| `<`, `>`, `<=`, `>=` | `5 > 3` → `true` | Greater/Less comparisons |

💡 **Hint:** Always use `===` instead of `==` to avoid unexpected type conversions.

Example:
```js
console.log(5 == "5");  // true (because "5" is converted to number)
console.log(5 === "5"); // false (different types)
```

#### **Logical Operators**  
| Operator | Example | Meaning |
|----------|----------|---------|
| `&&` | `true && false` → `false` | AND |
| `||` | `true || false` → `true` | OR |
| `!` | `!true` → `false` | NOT |

Example:
```js
let a = true, b = false;
console.log(a && b);  // false
console.log(a || b);  // true
console.log(!a);  // false
```

#### **Ternary Operator** (Shortcut for `if...else`)
```js
let age = 20;
let status = (age >= 18) ? "Adult" : "Minor";
console.log(status); // "Adult"
```
💡 **Hint:** `===` checks **both** value and type, while `==` converts types before comparison. Always use `===` unless you **intend** type coercion.

---

### **Home Exercise**  
- Swap two numbers **without using a third variable**.  
- Convert a string to a number and vice versa using JavaScript functions.  
- Use the **ternary operator** to check if a number is **even or odd**.  

---
