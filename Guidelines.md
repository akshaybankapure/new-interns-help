# Junior Developer Guidelines

## Brief
This document outlines coding, Git, and best practice guidelines for junior developers. It serves as a long-term reference for maintaining code quality, consistency, and efficiency in all projects. Follow these best practices to ensure seamless collaboration and maintainability.

---

## Learn More
- **Python Best Practices:** [Python PEP 8 Style Guide](https://peps.python.org/pep-0008/)
- **JavaScript Best Practices:** [JavaScript.info](https://javascript.info/)
- **TypeScript Handbook:** [TypeScript Docs](https://www.typescriptlang.org/docs/)
- **Git Best Practices:** [Atlassian Git Guide](https://www.atlassian.com/git/tutorials)
- **Commit Message Guidelines:** [Conventional Commits](https://www.conventionalcommits.org/)
- **Code Formatting:** [Prettier](https://prettier.io/) | [Black (Python)](https://black.readthedocs.io/en/stable/)
- **Cheat Sheets:**
  - [Python Cheatsheet](https://gto76.github.io/python-cheatsheet/)
  - [JavaScript Cheatsheet](https://htmlcheatsheet.com/js/)
  - [TypeScript Cheatsheet](https://typescript-cheatsheets.dev/)
  - [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

---

## Python Development Guidelines
- **Follow PEP 8** for coding style.
- **Use snake_case** for variables and functions.
- **Use PascalCase** for class names.
- **Type hints must be used** (`def func(x: int) -> str:`).
- **Keep imports structured** and **avoid circular dependencies**.
- **Ensure code readability** and maintain modular structure.
- **Example:**
  ```python
  class User:
      def __init__(self, name: str, age: int):
          self.name = name
          self.age = age
      
      def greet(self) -> str:
          return f"Hello, my name is {self.name}"
  ```

### Python Mini Cheat Sheet
| Concept  | Example  |
|----------|----------|
| List Comprehension | `[x**2 for x in range(10)]` |
| Dictionary Comprehension | `{x: x**2 for x in range(10)}` |
| Lambda Function | `square = lambda x: x * x` |
| Exception Handling | `try: ... except ValueError:` |

---

## JavaScript Development Guidelines
- **Use ES6+ syntax**.
- **Use const and let**, avoid var.
- **Follow camelCase** for variables and functions.
- **Use PascalCase** for class names.
- **Use modules** and avoid polluting the global scope.
- **Ensure async operations** do not block the event loop.
- **Example:**
  ```javascript
  class User {
      constructor(name, age) {
          this.name = name;
          this.age = age;
      }
      greet() {
          console.log(`Hello, my name is ${this.name}`);
      }
  }
  ```

### JavaScript Mini Cheat Sheet
| Concept  | Example  |
|----------|----------|
| Arrow Function | `const add = (a, b) => a + b` |
| Template Literals | ``Hello, ${name}!`` |
| Destructuring | `const { name, age } = user` |
| Promises | `fetch(url).then(res => res.json())` |

---

## Git Commit & Branch Naming
### Feature Branch Naming
```
feature/<JIRA-TICKET-ID>-<short-description>
```
**Example:**
```bash
feature/TCG-123-add-user-authentication
```

### Commit Messages
**Format:**
```bash
<type>: <short summary>

[Optional] Longer description if needed

[JIRA-TICKET-ID]
```
**Commit Types:**
- **feat**: New feature
- **fix**: Bug fix
- **chore**: Maintenance changes (dependencies, cleanup)
- **docs**: Documentation updates
- **test**: Adding/updating tests
- **refactor**: Code refactoring without behavior changes

**Example:**
```bash
feat: add user authentication

Implemented JWT-based authentication system.

TCG-123
```

---

## File Naming Conventions

### Python
- Modules: `module_name.py`
- Classes: `ClassName`
- Scripts: `script_name.py`

### JavaScript / TypeScript
- Components: `ComponentName.tsx`
- Services: `serviceName.ts`
- Utilities: `utilName.ts`
- Styles: `component-name.module.css`
- Configurations: `config.ts`
- Constants: `constants.ts`

---

## Module & Class Naming

### Python
- Modules: `snake_case`
- Classes: `PascalCase`
- Methods & Functions: `snake_case`

### JavaScript / TypeScript
- Module names: `camelCase`
- Class names: `PascalCase`
- Function names: `camelCase`

---

## Best Practices Summary
- **Write reusable, modular code**.
- **Use linters and formatters** (`ESLint`, `Prettier`, `Black`, `Flake8`).
- **Use meaningful logs and error messages**.
- **Document APIs and public functions**.
- **Use dependency management properly** (`package.json`, `requirements.txt`).
- **Test code before pushing** (`unit tests, integration tests`).
- **Follow Git workflow best practices** (`rebase, merge, conflict resolution`).

---

This document serves as a reference for all future developers to follow standardized and up-to-date coding practices.
