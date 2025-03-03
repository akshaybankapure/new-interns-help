# **Week 3: JavaScript Basics & Advanced Concepts**

## **Goal**
To build a **solid foundation** in JavaScript by covering both **basic and advanced topics**, ensuring hands-on practice, and providing **hints** to avoid roadblocks. The intern will complete **two learning sessions per day**, followed by an **at-home exercise** for reinforcement to maintain continuous engagement.

---

## **📅 Day 1: JavaScript Syntax, Variables & Operators**

### **Concepts to Learn**
- Setting up JavaScript (`<script>` tag & `console.log()`) ([W3Schools: JavaScript Introduction](https://www.w3schools.com/js/js_intro.asp))
- Declaring variables (`var`, `let`, `const`) and their scope ([MDN: Variables](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#variables))
- Understanding Hoisting ([MDN: Hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting))
- Primitive data types (`String`, `Number`, `Boolean`, `Null`, `Undefined`, `Symbol`, `BigInt`)
- Type coercion & conversions ([W3Schools: JavaScript Type Conversion](https://www.w3schools.com/js/js_type_conversion.asp))

💡 **Hint:** Use `typeof` to check data types in the console. **Be careful!** `typeof null` returns `"object"`—this is a JavaScript bug!

### **Concepts to Learn**
- Arithmetic Operators (`+`, `-`, `*`, `/`, `%`, `**`)
- Comparison Operators (`==`, `===`, `!=`, `!==`, `<`, `>`, `<=`, `>=`)
- Logical Operators (`&&`, `||`, `!`)
- Assignment Operators (`=`, `+=`, `-=`, `*=`, `/=`)
- Ternary Operator ([MDN: Conditional Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator))

💡 **Hint:** `===` is strict equality, while `==` does type conversion before comparison. **Avoid `==` unless necessary!**

### **Home Exercise**
- Swap two numbers without using a third variable.
- Convert a string to a number and vice versa using JavaScript functions.
- Use the ternary operator to check if a number is even or odd.

---
## **📅 Day 2: Control Flow, Loops & Functions**

### **Concepts to Learn**
- Conditional Statements (`if`, `else if`, `else`, `switch`)
- Looping Structures (`for`, `while`, `do...while`)
- Breaking out of loops (`break`, `continue`)
- Function Declarations vs Function Expressions
- Arrow Functions (`=>` syntax) and `this` behavior
- Default Parameters in Functions
- Higher-Order Functions (`map`, `filter`, `reduce`)
- Callback Functions

💡 **Hint:** Prefer arrow functions for short, simple functions, but use regular functions if `this` is needed.

### **Practice Exercises (Work Tasks)**
- Write a function that determines if a given number is prime.
- Implement a function that counts the number of vowels in a given string.
- Create a function that removes duplicate values from an array.

### **Fun Task** 🎉
- Build an interactive number guessing game.
- Create a rock-paper-scissors game against the computer.

### **More Practice**
- Implement a function that calculates the factorial of a number.
- Write a program that generates a random password of a given length.

### **More Fun Tasks** 🎉
- Create a function that checks if a string is a palindrome.
- Build a simple calculator using functions.

### **Home Exercises**
1. Write a function that takes a number and returns whether it is even or odd using both `if-else` and the ternary operator.
2. Create a function that takes a number and prints the multiplication table up to 10 using a `for` loop.
3. Write a function that simulates a simple banking system where a user can `deposit`, `withdraw`, and `check balance` using switch-case.
4. Implement a function that finds and returns the largest number in an array.
5. Create a function that accepts a list of words and returns a new list with only the words that have more than 5 letters.

---

## **📅 Day 3: Arrays & Objects**

### **Concepts to Learn**
- Creating and Modifying Arrays (`push`, `pop`, `shift`, `unshift`)
- Iterating Over Arrays (`map`, `filter`, `reduce`, `forEach`)
- Sorting and Searching in Arrays (`sort`, `find`, `indexOf`, `includes`)
- Object Literals & Accessing Properties
- Adding & Removing Properties in Objects
- Object Destructuring & Spread Operator (`...`)

💡 **Hint:** Use `map` when you need a new array, `forEach` when you just need to iterate.

### **Practice Exercises (Work Tasks)**
- Write a function that finds the largest number in an array.
- Create a function that flattens a nested array.
- Implement a function that returns a new object with only the specified properties.

### **Fun Task** 🎉
- Build a to-do list app where users can add, remove, and mark tasks as completed.
- Implement a function that merges two arrays and removes duplicates.

### **More Practice**
- Create an inventory system where objects represent items with properties like `name`, `price`, and `quantity`.
- Implement a function that sorts an array of student objects based on their grades.

### **More Fun Tasks** 🎉
- Build a simple shopping cart that calculates the total cost.
- Create a function that randomly shuffles an array.

### **Home Exercises**
1. Write a function that takes an array of numbers and returns a new array with only even numbers.
2. Create an object representing a student with `name`, `age`, `grade`, and `subjects` (array). Write functions to add a new subject, update the grade, and retrieve details.
3. Write a program that accepts a list of names and returns a list sorted in alphabetical order.
4. Implement a function that takes an array of numbers and returns an object containing the `sum`, `average`, `minimum`, and `maximum` values.
5. Create a function that accepts a list of book objects and filters out books published before the year 2000.

---

## **📅 Day 4: DOM Manipulation & Event Handling**

### **Concepts to Learn**
- Selecting Elements (`getElementById`, `querySelector`, `querySelectorAll`)
- Modifying Elements (`innerText`, `innerHTML`, `style`)
- Handling Forms (`value`, `submit` event, `preventDefault()`)
- Creating and Removing Elements (`createElement`, `appendChild`, `removeChild`)
- Handling Input Events (`keyup`, `change`, `focus`, `blur`)
- Event Propagation (`bubbling` & `capturing`)
- Event Delegation

💡 **Hint:** Use `event.target` to see which element triggered the event.

### **Practice Exercises (Work Tasks)**
- Create an interactive form that updates live as the user types.
- Implement a button that changes the page background color when clicked.
- Make a list where clicking an item removes it from the page.

### **Fun Task** 🎉
- Build a basic interactive calculator using buttons and input fields.
- Create an image gallery that changes images when clicking on thumbnails.

### **More Practice**
- Implement a simple light/dark mode toggle.
- Build a simple character counter that updates as the user types.

### **More Fun Tasks** 🎉
- Build a simple interactive stopwatch.
- Create an interactive rating system.

### **Home Exercises**
1. Create a form with `Name`, `Email`, and `Message` fields. Validate that all fields are filled before submission.
2. Implement a counter app that increments or decrements the number when buttons are clicked.
3. Create a dropdown that dynamically changes the page content when a selection is made.
4. Write a script where a button, when clicked, generates a new random number and displays it on the page.
5. Build a simple app that allows users to add their favorite books to a list and remove them when clicked.

---


## **📅 Day 5: DOM Manipulation & Forms Handling**

### **Concepts to Learn**
- Selecting Elements (`getElementById`, `querySelector`)
- Modifying Elements (`innerText`, `innerHTML`, `style`)
- Handling Forms (`value`, `submit` event, `preventDefault()`)
- Creating and Removing Elements (`createElement`, `appendChild`, `removeChild`)

💡 **Hint:** Use `document.querySelectorAll()` to select multiple elements at once.

### **Concepts to Learn**
- Handling Input Events (`keyup`, `change`, `focus`, `blur`)
- Event Propagation (`bubbling` & `capturing`)
- Event Delegation
- Callbacks & `setTimeout()` / `setInterval()`

💡 **Hint:** Use `event.target` to see which element triggered the event.

### **Home Exercise**
- Create an interactive form that updates live as the user types.
- Implement a button that changes the page background color when clicked.
- Make a list where clicking an item removes it from the page.

---

## **📅 Day 6: Error Handling & Debugging**

### **Concepts to Learn**
- Using `try...catch...finally`
- Throwing custom errors (`throw` statement)
- Handling asynchronous errors (`try-catch` in async functions)
- Debugging with `console.log()`, `console.error()`, and browser dev tools

💡 **Hint:** Use `debugger;` in your code to create breakpoints when debugging.

### **Concepts to Learn**
- The Call Stack and Event Loop ([MDN: Call Stack](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack))
- Understanding Asynchronous JavaScript (`setTimeout`, `setInterval`)
- How `Promises` work (basic introduction)

💡 **Hint:** A Promise is a placeholder for an eventual result. Use `.then()` to handle success and `.catch()` for errors.

### **Home Exercise**
- Simulate a delayed API response using `setTimeout()`.
- Write a function that retries a failed operation up to three times before throwing an error.
- Log all errors in a structured way using `console.error()`.

---

## **📅 Day 7: JavaScript Best Practices & Project Wrap-up**

### **Concepts to Learn**
- Code Formatting & Linting (`Prettier`, `ESLint`)
- Writing Clean & Readable Code
- Avoiding Common JavaScript Mistakes
- Performance Optimization Techniques

💡 **Hint:** Use **`const`** by default and only use **`let`** if the value needs to change.

### **Concepts to Learn**
- Organizing JavaScript Code (Single Responsibility Principle)
- Importance of Comments & Documentation
- JavaScript Performance Optimization
- Introduction to JavaScript Modules (`import` / `export`)

💡 **Hint:** Split code into small reusable functions instead of one large function.

### **Home Exercise**
- Review and optimize a messy JavaScript file by applying best practices.
- Convert an existing script into a modular format using `import/export`.
- Prepare a mini-presentation on key JavaScript best practices.

---
