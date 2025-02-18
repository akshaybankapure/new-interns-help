# Guide to Using Environment Variables in Python

## What are Environment Variables?
Environment variables are dynamic values that the operating system or a program can use to influence the behavior of processes. They are commonly used to store configuration settings, secrets, API keys, or other sensitive information.

## Why Use Environment Variables?
1. **Security**: Keeps sensitive information (like API keys) out of the codebase.
2. **Flexibility**: Allows changing configurations without modifying the source code.
3. **Portability**: Ensures the program can run in different environments (development, staging, production) without changing code.

---
## Different Ways to Use Environment Variables in Python
There are multiple ways to handle environment variables in Python. Choosing the right method depends on the use case.


### 1. Using a `.env` File with `python-dotenv` (preferred)
Best suited for:
- Managing multiple environment variables.
- Keeping secrets and configuration separate from code.
- Loading settings dynamically in different environments (dev, test, production).

#### Step 1: Install `python-dotenv`
```sh
pip install python-dotenv
```

#### Step 2: Create a `.env` File
```env
TASK_MANAGER_MODE=development
DB_PATH=tasks.json
```

#### Step 3: Load the `.env` File in Python
```python
from dotenv import load_dotenv
import os

# Load variables from .env file
load_dotenv()

# Access environment variables
db_path = os.getenv('DB_PATH', 'default_tasks.json')
print(f"Using database: {db_path}")
```
**When NOT to use:**
- If the application is running in a containerized or cloud environment where secret managers are available (AWS Secrets Manager, Kubernetes Secrets, etc.).

### 2. Using `os.environ` (Direct Environment Variables)
Best suited for:
- Temporary environment variables within the session.
- Simple configurations that do not need persistence.

Example:
```python
import os

# Set an environment variable (only for the current session)
os.environ['TASK_MANAGER_MODE'] = 'development'

# Retrieve an environment variable
mode = os.getenv('TASK_MANAGER_MODE', 'production')  # Default to 'production' if not set
print(f"Running in {mode} mode")
```
**When NOT to use:**
- When environment variables need to persist across sessions.
- When storing secrets (prefer .env files or system environment variables).


### 3. Using System-Level Environment Variables
Best suited for:
- Production environments where secrets should not be stored in a `.env` file.
- Applications running in CI/CD pipelines, Docker, or cloud deployments.

Example:
Set an environment variable in Linux/macOS:
```sh
export TASK_MANAGER_MODE=production
```
Set an environment variable in Windows (Command Prompt):
```sh
set TASK_MANAGER_MODE=production
```
Retrieve it in Python:
```python
import os
mode = os.getenv('TASK_MANAGER_MODE')
print(f"Running in {mode} mode")
```
**When NOT to use:**
- When working in a local development setup where frequent changes are needed.

---
## Implementing Environment Variables in the CLI Task Manager

### 1. Storing Task Manager Configuration
Create a `.env` file in the `task_manager/` directory:
```env
TASK_STORAGE_FILE=tasks.json
LOG_LEVEL=debug
```

### 2. Loading Environment Variables in `storage.py`
Modify `storage.py` to use environment variables:
```python
from dotenv import load_dotenv
import os
import json

# Load environment variables
load_dotenv()

# Get storage file path
db_file = os.getenv('TASK_STORAGE_FILE', 'tasks.json')

def load_tasks():
    """ Load tasks from the JSON file. """
    try:
        with open(db_file, 'r') as file:
            return json.load(file)
    except (FileNotFoundError, json.JSONDecodeError):
        return []

def save_tasks(tasks):
    """ Save tasks to the JSON file. """
    with open(db_file, 'w') as file:
        json.dump(tasks, file, indent=4)
```

### 3. Using Context Managers (with Statement) in Task Handling
A context manager ensures that files are properly opened and closed, reducing the risk of resource leaks.
Modify `storage.py` to use a context manager:
```python
def load_tasks():
    """ Load tasks using a context manager """
    try:
        with open(db_file, 'r') as file:
            return json.load(file)
    except (FileNotFoundError, json.JSONDecodeError):
        return []

def save_tasks(tasks):
    """ Save tasks using a context manager """
    with open(db_file, 'w') as file:
        json.dump(tasks, file, indent=4)
```

### 4. Using Environment Variables for Logging
Modify `main.py` to configure logging level using environment variables:
```python
import os
import logging
from dotenv import load_dotenv

# Load environment variables
load_dotenv()

# Set logging level
log_level = os.getenv('LOG_LEVEL', 'info').upper()
logging.basicConfig(level=getattr(logging, log_level, logging.INFO))

logging.info("Task Manager Started")
```

---
### Conclusion
Using environment variables in Python ensures that configurations remain secure, flexible, and easy to change without modifying code. Different methods should be used based on the environment and requirements:
- `os.environ` for temporary or simple setups.
- `.env` files with `python-dotenv` for local development.
- System-level environment variables for production and containerized deployments.
This approach enhances the usability and maintainability of the CLI Task Manager.









### Example:

```python
import json
import argparse
from pathlib import Path

# Define the file path for task storage
TASK_FILE = Path("tasks.json")

# Storage Management
class Storage:
    @staticmethod
    def load_tasks():
        if TASK_FILE.exists():
            with open(TASK_FILE, "r") as file:
                return json.load(file)
        return {"tasks": []}

    @staticmethod
    def save_tasks(tasks):
        with open(TASK_FILE, "w") as file:
            json.dump(tasks, file, indent=4)

# Task Handling
class TaskManager:
    def __init__(self):
        self.tasks = Storage.load_tasks()
    
    def add_task(self, description):
        self.tasks["tasks"].append({"description": description, "completed": False})
        Storage.save_tasks(self.tasks)
        print(f"Task added: {description}")
    
    def remove_task(self, index):
        try:
            task = self.tasks["tasks"].pop(index)
            Storage.save_tasks(self.tasks)
            print(f"Task removed: {task['description']}")
        except IndexError:
            print("Invalid task index.")
    
    def list_tasks(self, completed=None):
        for idx, task in enumerate(self.tasks["tasks"]):
            if completed is None or task["completed"] == completed:
                status = "✓" if task["completed"] else "✗"
                print(f"[{idx}] {status} {task['description']}")
    
    def mark_completed(self, index):
        try:
            self.tasks["tasks"][index]["completed"] = True
            Storage.save_tasks(self.tasks)
            print(f"Task marked as completed: {self.tasks['tasks'][index]['description']}")
        except IndexError:
            print("Invalid task index.")

# Command-Line Interface Integration
def main():
    parser = argparse.ArgumentParser(description="CLI Task Manager")
    parser.add_argument("--add", metavar="task", type=str, help="Add a new task")
    parser.add_argument("--remove", metavar="index", type=int, help="Remove a task by index")
    parser.add_argument("--list", action="store_true", help="List all tasks")
    parser.add_argument("--completed", action="store_true", help="List only completed tasks")
    parser.add_argument("--pending", action="store_true", help="List only pending tasks")
    parser.add_argument("--done", metavar="index", type=int, help="Mark task as completed")
    
    args = parser.parse_args()
    manager = TaskManager()
    
    if args.add:
        manager.add_task(args.add)
    elif args.remove is not None:
        manager.remove_task(args.remove)
    elif args.list:
        manager.list_tasks()
    elif args.completed:
        manager.list_tasks(completed=True)
    elif args.pending:
        manager.list_tasks(completed=False)
    elif args.done is not None:
        manager.mark_completed(args.done)
    else:
        parser.print_help()

if __name__ == "__main__":
    main()

```


