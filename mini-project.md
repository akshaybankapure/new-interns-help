# **Guided Mini Project: Engineering Standard Practices in Software Development**

## **Overview**
This guided project introduces **engineering standard practices** by following a modular and scalable approach. The intern will build a **task management system** using **Vite, JavaScript, and Object-Oriented Programming (OOP) principles** such as **inheritance, constructors, method overloading, encapsulation, and modular design**.
This also ensures that the person learns **industry-standard software development practices** while actively contributing new features **in a structured workflow**. 🚀

By completing this project, the intern will:
- Learn **how to structure a project properly**.
- Follow **best practices in modularization, file structure, and documentation**.
- Implement **OOP concepts** in JavaScript.
- Understand **how to work with Vite for fast development**.
- Use **ES6 modules, dependency injection, and testing best practices**.
- Follow **proper Git workflow** by raising **Pull Requests (PRs)** before merging new features.

---

## **📌 Project Overview: Task Management System**
The Task Management System will allow users to **create, update, delete, and filter tasks**, following engineering principles such as **scalability, maintainability, and reusability**.

### **📂 Folder Structure (Following Engineering Standards)**
```
task-manager/
├── src/
│   ├── components/
│   │   ├── Task.js  # Task class (OOP principles: encapsulation, constructors, inheritance)
│   │   ├── TaskList.js  # Manages tasks using Task class
│   │   ├── UI.js  # Handles user interactions and rendering
│   │   ├── Storage.js  # Handles LocalStorage for task persistence
│   ├── utils/
│   │   ├── helpers.js  # Utility functions
│   ├── styles/
│   │   ├── main.css  # Styles for UI
│   ├── main.js  # Entry point (initialize app)
├── index.html  # Main HTML file
├── vite.config.js  # Configuration for Vite
├── package.json  # Project dependencies
├── README.md  # Project documentation
```

---

## **🔹 Setting Up Vite for the Project**
1. Install Vite and create a new project:
   ```sh
   npm create vite@latest task-manager --template vanilla
   cd task-manager
   npm install
   ```
2. Run the development server:
   ```sh
   npm run dev
   ```
3. Open the browser at `http://localhost:5173/` to see your project running.

---

## **🟢 Step 1: Creating the `Task` Class (Encapsulation & Constructors)**
Each task should have:
- **A unique ID** (generated automatically).
- **A title**.
- **A description**.
- **A status** (Pending, Completed).
- **A due date**.

### **📌 `Task.js` (Encapsulation & Constructors)**
```js
export class Task {
  constructor(title, description, dueDate) {
    this.id = Date.now();
    this.title = title;
    this.description = description;
    this.dueDate = dueDate;
    this.status = "Pending";
  }

  markCompleted() {
    this.status = "Completed";
  }
}
```
💡 **Best Practice:** Encapsulate task properties within a class and use methods to modify them.

---

## **🔹 Additional Features for the Intern to Implement**
After setting up the project, the intern should contribute by implementing the following features **one at a time**, following the Git workflow outlined below.

### **Git Workflow for Every Feature Implementation**
1. **Create a new feature branch** from `main` before starting any new feature:
   ```sh
   git checkout main
   git pull origin main
   git checkout -b feature-<feature-name>
   ```
2. **Work on the feature and commit changes regularly.**
3. **Push the feature branch to GitHub:**
   ```sh
   git push origin feature-<feature-name>
   ```
4. **Raise a Pull Request (PR) to merge changes into `main` and wait for approval.**
5. **Merge the PR once approved.**
6. **Switch back to `main`, pull the latest changes, and create a new feature branch for the next task:**
   ```sh
   git checkout main
   git pull origin main
   git checkout -b feature-next-feature
   ```

---

### **Features for the Intern to Implement**

### **1️⃣ Feature: Task Categories**
- Modify `Task.js` to include a `category` property.
- Add predefined categories like `Work`, `Personal`, `Urgent`.

### **2️⃣ Feature: Task Priority Levels**
- Implement priority levels (`Low`, `Medium`, `High`).
- Extend `UrgentTask.js` to include priority logic.

### **3️⃣ Feature: Task Deadlines & Reminders**
- Use `setTimeout()` to notify when a task is near its deadline.
- Display overdue tasks differently in the UI.

### **4️⃣ Feature: Task Filtering by Status**
- Modify `TaskList.js` to filter tasks by **Pending**, **Completed**, **Overdue**.

### **5️⃣ Feature: Task Search Functionality**
- Add a search bar to filter tasks dynamically as the user types.

### **6️⃣ Feature: Drag and Drop Tasks**
- Implement drag-and-drop functionality for sorting tasks visually.

### **7️⃣ Feature: Task Persistence via API (instead of LocalStorage)**
- Replace `Storage.js` with a REST API backend.
- Implement **fetch()** to save and retrieve tasks from a server.

### **8️⃣ Feature: Dark Mode Toggle**
- Add a UI toggle for switching between light and dark modes.

### **9️⃣ Feature: Notifications on Task Updates**
- Use the Notification API or toast popups when tasks are added/removed.

### **🔟 Feature: Unit Testing**
- Write unit tests for `Task.js` and `TaskList.js` using Jest.
- Ensure all methods work as expected.

---

## **✅ Summary of Engineering Best Practices Followed**
✔ **Modularization:** Code is split into **separate files**.
✔ **OOP Principles:** Classes, Inheritance, Encapsulation, and Overriding.
✔ **Data Persistence:** Uses `localStorage` or REST API.
✔ **Event Handling:** Handles user interactions via UI.js.
✔ **Scalability:** Easily extendable (e.g., authentication, API integration).
✔ **Code Reusability:** Methods follow the **Single Responsibility Principle (SRP)**.
✔ **Testing:** Encourages TDD with Jest for maintainability.
✔ **Git Workflow:** Uses feature branching, PR approvals, and merging best practices.

---
