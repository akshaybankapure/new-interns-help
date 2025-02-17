# **Week 2: Intermediate Python & Backend Development**

## **Goal**
Build on Python fundamentals by introducing **advanced data structures, file handling, object-oriented programming (OOP), error handling, and an introduction to FastAPI** for backend development. The intern will work on **real-world API implementations** with modular design, proper error handling, and **industry-standard best practices** such as environment variables, logging, and security. The focus will be on **progressively building a backend system** step by step, each day contributing to a growing **modular, scalable project**.

---

## **📅 Day 1: Advanced Data Structures, File Handling & Industry Standards**

### **Concepts to Learn**
- **Advanced Lists**: Sorting with key functions, list slicing techniques ([W3Schools: Lists](https://www.w3schools.com/python/python_lists.asp))
- **Dictionary Operations**: Nested dictionaries, dictionary comprehensions ([W3Schools: Dictionaries](https://www.w3schools.com/python/python_dictionaries.asp))
- **Set Operations**: Unions, intersections, and differences ([W3Schools: Sets](https://www.w3schools.com/python/python_sets.asp))
- **File Handling**: Reading and writing files, working with CSV and JSON ([W3Schools: File Handling](https://www.w3schools.com/python/python_file_handling.asp))
- **Context Managers (`with` statement)** for efficient file handling ([Python Docs](https://docs.python.org/3/library/contextlib.html))
- **Environment Variables (`.env` files)** for managing secrets and configurations ([12-Factor App Guidelines](https://12factor.net/config))

### **🔥 Major Exercise: User Data Storage System**
- Create a **user data storage module** that reads/writes user information to a **CSV file**.
- Implement functions for **adding, updating, deleting, and retrieving user records**.
- Store file paths and configurations using a **`.env` file**.
- Use **context managers** to ensure proper file handling.

---

## **📅 Day 2: Object-Oriented Programming (OOP) & Modular Code Design**

### **Concepts to Learn**
- **Classes & Objects** ([W3Schools: OOP](https://www.w3schools.com/python/python_classes.asp))
- **Encapsulation, Inheritance & Polymorphism**
- **Dunder Methods (`__str__`, `__repr__`, `__eq__`)**
- **Class vs. Instance Attributes**
- **Abstract Classes & Interfaces (`ABC` module)** ([Python Docs](https://docs.python.org/3/library/abc.html))
- **Why Modular Programming Matters?** ([Software Engineering Best Practices](https://martinfowler.com/))

### **🔥 Major Exercise: User Management Class System**
- Convert the **User Data Storage System** into a **fully object-oriented system**.
- Implement a **User class** with methods for managing user information.
- Use **inheritance** to create an `AdminUser` class with additional permissions.
- Store user objects in a **JSON file** instead of CSV for structured storage.

---

## **📅 Day 3: Error Handling, Logging & Debugging Industry Standards**

### **Concepts to Learn**
- **Exception Handling (`try-except-finally`)** ([W3Schools: Errors](https://www.w3schools.com/python/python_try_except.asp))
- **Custom Exceptions (`raise` & `assert`)**
- **Logging (`logging` module) for Debugging & Production Environments** ([Python Docs](https://docs.python.org/3/library/logging.html))
- **Handling Multiple Exceptions & Nested Try Blocks**
- **Why Logging is Critical in Industry?** ([Best Practices](https://realpython.com/python-logging/))

### **🔥 Major Exercise: Enhanced User Management with Logging**
- Implement **error handling** in the **User Management System**.
- Add **logging** to track **user actions and system errors**.
- Store logs in a **rotating log file** for better debugging.

---

## **📅 Day 4-7: FastAPI & Backend Development**

### **Concepts to Learn**
- **Setting Up FastAPI** ([FastAPI Docs](https://fastapi.tiangolo.com/))
- **Creating Modular API Routes (`@app.get`, `@app.post`)**
- **Pydantic Models for Data Validation** ([Pydantic Docs](https://pydantic-docs.helpmanual.io/))
- **JWT Authentication & Security Best Practices** ([FastAPI Security](https://fastapi.tiangolo.com/advanced/security/))
- **Database Connection (SQLite/PostgreSQL) using SQLAlchemy** ([SQLAlchemy Docs](https://docs.sqlalchemy.org/en/14/))
- **Middleware & Dependency Injection** ([Best Practices](https://fastapi.tiangolo.com/tutorial/dependencies/))
- **Containerization & Deployment with Docker** ([Docker Docs](https://docs.docker.com/get-started/))

### **🔥 Major Exercise: FastAPI-Powered User Management System**
- Convert the **OOP-based User Management System** into a **REST API using FastAPI**.
- Implement **CRUD operations** for user data with **FastAPI endpoints**.
- Validate input using **Pydantic models**.
- Implement **JWT-based authentication** for secure user login.
- Store user data in **PostgreSQL/SQLite**.
- Add **middleware for logging API requests and responses**.
- Deploy the service **inside a Docker container**.

---

## **Final Git Task**
- Create a feature branch **`feature-scalable-backend`**.
- Implement **modular commits** for each day's enhancement.
- **Document the API using FastAPI’s built-in Swagger UI.**
- **Merge after review.**

---

### **Outcome**
By the end of this week, the intern will have built a **complete backend system** that follows **industry standards, modular programming, API design, authentication, error handling, logging, and containerization**. This growing project will serve as a **practical portfolio piece** demonstrating real-world backend development skills. 🚀

