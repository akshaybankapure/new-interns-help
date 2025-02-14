# Junior Developer Guidelines

## General Development Guidelines
- **Write Readable Code:** Follow clean code principles and write self-explanatory code.
- **Follow DRY & SOLID Principles:** Avoid code duplication and ensure modularity.
- **Use Proper Naming Conventions:** Variables, functions, and classes should have meaningful names.
- **Write Unit Tests:** Ensure your code is covered with unit tests.
- **Code Reviews:** Always submit a pull request for review before merging.
- **Error Handling:** Implement proper error handling and logging.
- **Security:** Follow security best practices to prevent vulnerabilities.
- **Documentation:** Add meaningful comments and update documentation when necessary.
- **Version Control:** Use Git properly, follow branching strategies, and write meaningful commit messages.

---

## Typing Guidelines

### JavaScript (JS)
- Prefer **ES6+ syntax**.
- Use **const** and **let**, avoid **var**.
- Follow **camelCase** for variables and functions.
- Use **PascalCase** for class names.
- Use **modules** and avoid polluting the global scope.
- Ensure code **does not block the event loop unnecessarily**.

### TypeScript (TS)
- Use **strict types**.
- Define **interfaces and types** instead of using `any`.
- Prefer **readonly properties** where applicable.
- Always define function return types.
- Keep TypeScript **configurations strict** (`strict: true`).

### Python
- Follow **PEP 8** for styling.
- Use **snake_case** for variables and functions.
- Use **PascalCase** for class names.
- Type hints **must be used** (`def func(x: int) -> str:`).
- Keep imports **structured** and **avoid circular dependencies**.

---

## Git Commit & Branch Naming

### Feature Branch Naming
`feature/<JIRA-TICKET-ID>-<short-description>`

Example:
```bash
feature/TCG-123-add-user-authentication
```

### Commit Messages
Format:
```bash
<type>: <short summary>

[Optional] Longer description if needed

[JIRA-TICKET-ID]
```

Types:
- **feat**: New feature
- **fix**: Bug fix
- **chore**: Maintenance changes (dependencies, cleanup)
- **docs**: Documentation updates
- **test**: Adding/updating tests
- **refactor**: Code refactoring without behavior changes

Example:
```bash
feat: add user authentication

Implemented JWT-based authentication system.

TCG-123
```

---

## File Naming Conventions

### JavaScript / TypeScript
- Components: `ComponentName.tsx`
- Services: `serviceName.ts`
- Utilities: `utilName.ts`
- Styles: `component-name.module.css`
- Configurations: `config.ts`
- Constants: `constants.ts`

### Python
- Modules: `module_name.py`
- Classes: `ClassName`
- Scripts: `script_name.py`

---

## Module & Class Naming

### JavaScript / TypeScript
- Module names: `camelCase`
- Class names: `PascalCase`
- Function names: `camelCase`

### Python
- Modules: `snake_case`
- Classes: `PascalCase`
- Methods & Functions: `snake_case`

---

## Best Practices Summary
- **Write reusable, modular code**.
- **Use linters and formatters** (`ESLint`, `Prettier`, `Black`, `Flake8`).
- **Use meaningful logs and error messages**.
- **Document APIs and public functions**.
- **Use dependency management properly** (`package.json`, `requirements.txt`).
- **Test code before pushing** (`unit tests, integration tests`).
