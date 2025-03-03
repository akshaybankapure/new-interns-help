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
- [Conditional Statements (`if`, `else if`, `else`, `switch`)](https://www.w3schools.com/js/js_if_else.asp)
- [Looping Structures (`for`, `while`, `do...while`)](https://www.w3schools.com/js/js_loop_for.asp)
- [Breaking out of loops (`break`, `continue`)](https://www.w3schools.com/js/js_loop_for.asp#loopbreak)
- [Function Declarations vs Function Expressions](https://www.w3schools.com/js/js_function_definition.asp)
- [Arrow Functions (`=>` syntax) and `this` behavior](https://www.w3schools.com/js/js_arrow_function.asp)
- [Default Parameters in Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Default_parameters)
- [Higher-Order Functions (`map`, `filter`, `reduce`)](https://www.w3schools.com/js/js_array_iteration.asp)
- [Callback Functions](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)


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
- [Creating and Modifying Arrays (`push`, `pop`, `shift`, `unshift`)](https://www.w3schools.com/js/js_array_methods.asp)
- [Iterating Over Arrays (`map`, `filter`, `reduce`, `forEach`)](https://www.w3schools.com/js/js_array_iteration.asp)
- [Sorting and Searching in Arrays (`sort`, `find`, `indexOf`, `includes`)](https://www.w3schools.com/js/js_array_sort.asp)
- [Object Literals & Accessing Properties](https://www.w3schools.com/js/js_objects.asp)
- [Adding & Removing Properties in Objects](https://www.w3schools.com/js/js_objects.asp)
- [Object Destructuring & Spread Operator (`...`)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)

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
- [Selecting Elements (`getElementById`, `querySelector`, `querySelectorAll`)](https://www.w3schools.com/js/js_htmldom_elements.asp)
- [Modifying Elements (`innerText`, `innerHTML`, `style`)](https://www.w3schools.com/js/js_htmldom_html.asp)
- [Handling Forms (`value`, `submit` event, `preventDefault()`)](https://www.w3schools.com/js/js_validation.asp)
- [Creating and Removing Elements (`createElement`, `appendChild`, `removeChild`)](https://www.w3schools.com/js/js_htmldom_nodes.asp)
- [Handling Input Events (`keyup`, `change`, `focus`, `blur`)](https://www.w3schools.com/jsref/event_onkeyup.asp)
- [Event Propagation (`bubbling` & `capturing`)](https://www.w3schools.com/jsref/event_bubbles.asp)
- [Event Delegation](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)


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

## **📅 Day 5: Asynchronous JavaScript & Fetch API**

### **Concepts to Learn**
- [Understanding Asynchronous JavaScript](https://www.w3schools.com/js/js_asynchronous.asp) (`setTimeout`, `setInterval`)
- [JavaScript Callbacks & Promises](https://www.w3schools.com/js/js_promise.asp) (`.then`, `.catch`)
- [async and await](https://www.w3schools.com/js/js_async.asp)
- [Fetch API](https://www.w3schools.com/js/js_api_fetch.asp) (`fetch`, `JSON.parse()`)
- [Handling API Errors](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) (`try...catch` with `fetch`)

💡 **Hint:** A Promise is a placeholder for an eventual result. Use `.then()` to handle success and `.catch()` for errors.

### **Practice Exercises (Work Tasks)**
- Use `setTimeout()` to log a message after 3 seconds.
- Create a function that returns a Promise which resolves after 2 seconds.
- Implement an API call using `fetch()` to retrieve data from a public API.

### **Fun Task** 🎉
- Build a simple joke generator that fetches random jokes from an API.
- Create a mini weather app that fetches weather data based on user input.

### **More Practice**
- Write a function that fetches data from an API and logs only specific properties.
- Implement a retry mechanism for API requests that fail.

### **More Fun Tasks** 🎉
- Build a currency converter that fetches exchange rates from an API.
- Create a GitHub user search tool that fetches profile details from the GitHub API.

### **Home Exercises**
1. Fetch and display user data from the [JSONPlaceholder API](https://jsonplaceholder.typicode.com/).
2. Implement a function that makes multiple API calls sequentially.
3. Create a function that fetches an API response, modifies the data, and displays it on the webpage.
4. Implement error handling when making an API call using `try...catch`.
5. Write a function that fetches data every 10 seconds and updates the webpage.

---

## **📅 Day 6: Error Handling, Debugging & Local Storage**

### **Concepts to Learn**
- [Using `try...catch...finally`](https://www.w3schools.com/js/js_errors.asp)
- [Throwing custom errors (`throw` statement)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/throw)
- [Debugging with `console.log()`, `console.error()`, and browser dev tools](https://www.w3schools.com/js/js_debugging.asp)
- [Using Local Storage](https://www.w3schools.com/jsref/prop_win_localstorage.asp) (`localStorage.setItem`, `getItem`, `removeItem`)
- [Session Storage & Cookies](https://developer.mozilla.org/en-US/docs/Web/API/Window/sessionStorage)

💡 **Hint:** Use `debugger;` in your code to create breakpoints when debugging.

### **Practice Exercises (Work Tasks)**
- Implement error handling in a function that calculates the square root of a number.
- Store and retrieve user settings using `localStorage`.
- Debug an existing script with intentional errors and fix them.

### **Fun Task** 🎉
- Build a persistent to-do list that saves tasks even after refreshing the page.
- Implement a theme switcher that remembers the user's preference using local storage.

### **More Practice**
- Create a login system that stores and retrieves user data from local storage.
- Implement a settings page where users can adjust preferences and store them in local storage.

### **More Fun Tasks** 🎉
- Build a small notes app that allows users to write, save, and delete notes using local storage.
- Create a countdown timer that persists time across page reloads using session storage.

### **Home Exercises**
1. Implement error handling for a function that fetches data from an API.
2. Create a local storage-based shopping cart that saves selected items.
3. Implement a simple bookmarking system that saves favorite links.
4. Debug a given JavaScript script and document all fixes made.
5. Build a simple app that remembers the last entered text input field data even after the page refreshes.

---

## **📅 Day 7: JavaScript Best Practices & Project Wrap-up**

### **Concepts to Learn**
- [Code Formatting & Linting](https://prettier.io/) (`Prettier`, `ESLint`)
- [Writing Clean & Readable Code](https://google.github.io/styleguide/jsguide.html)
- [Avoiding Common JavaScript Mistakes](https://www.w3schools.com/js/js_mistakes.asp)
- [Performance Optimization Techniques](https://developer.mozilla.org/en-US/docs/Web/Performance)
- [Event Delegation & Best Practices](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

💡 **Hint:** Use **`const`** by default and only use **`let`** if the value needs to change.

### **Practice Exercises (Work Tasks)**
- Review and optimize a messy JavaScript file by applying best practices.
- Refactor an existing script to improve readability and maintainability.
- Implement event delegation for dynamically added elements.

### **Fun Task** 🎉
- Build a small interactive quiz that asks JavaScript-related questions and provides feedback.
- Create a simple memory game that uses JavaScript to track clicked items.

### **More Practice**
- Implement a feature that improves performance in an existing script.
- Debug and analyze slow-performing JavaScript code.

### **More Fun Tasks** 🎉
- Develop a lightweight stopwatch using JavaScript and the `setInterval()` function.
- Make a **mini JavaScript project** using everything learned so far. Example ideas:
  - A task manager
  - A notes app
  - A budget calculator
  - A personal expense tracker
  - A habit tracker

### **Home Exercises**
1. Optimize a given JavaScript function to run more efficiently.
2. Write a script that logs JavaScript errors and saves them for debugging.
3. Implement event delegation in a list where new items can be dynamically added.
4. Build a lightweight search filter that filters data as the user types.
5. Create a JavaScript style guide document listing best practices.

---

## **📅 WeekEnds Optional1: DOM Manipulation & Forms Handling**

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
