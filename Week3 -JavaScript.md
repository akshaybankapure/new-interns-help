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
