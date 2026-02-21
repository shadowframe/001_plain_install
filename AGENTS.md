# AGENTS.md

## Purpose
This document serves as the central guide for all coding agents (including AI agents) contributing to this repository. It provides the essential commands and guidelines to ensure consistency and maintainability.

---

## Build, Lint, and Test Commands

### Build Commands
- **Start a development server:**
  ```bash
  npx vite
  ```
  This command spins up a Vite development server, serving the project on a local port.

### Test Commands
- **Testing Framework:** Currently, no specific testing framework is configured. Consider integrating a tool like Jest or Vitest for unit testing.

### Lint Commands
- **Linting Framework:** No specific linting framework is defined yet. Consider adding ESLint for code quality checks.

### Additional Suggestions
- Before pushing new changes, ensure that the app runs without errors in the development server.

---

## Code Style Guidelines

To maintain consistency, adhere to the following stylistic rules:

### Imports
- Use ES6 module imports:
  ```javascript
  import * as THREE from 'three';
  ```

### Formatting
- **Indentation:** Use 2 spaces for indentation.
- **Line Length:** Keep lines under 80 characters where possible.
- **Trailing Spaces and Newlines:** Avoid trailing spaces and ensure a newline at the end of files.

### Types
- **TypeScript:** Not currently used. If desired, recommend TypeScript for type safety in future work.

### Naming Conventions
- Use `camelCase` for variables and functions:
  ```javascript
  const myVariable = 42;
  function doSomething() {}
  ```
- Use `PascalCase` for class or component names:
  ```javascript
  class MyClass {}
  ```
- CONSTANT_VALUES should be in `SCREAMING_SNAKE_CASE` if applicable.

### Error Handling
- No specific error handling mechanism is currently implemented. Ensure any new additions include proper safety checks.
- For instance, validate critical inputs before using them:
  ```javascript
  if (!value) {
    throw new Error('Invalid value');
  }
  ```

### Comments
- Use descriptive comments to explain complex logic:
  ```javascript
  // Rotate cube based on time
  cube.rotation.x = time / 2000;
  ```

---

## Suggested Improvements

1. **Testing Setup:**
   - Add a testing framework like Jest or Vitest.
2. **Linting:**
   - Configure ESLint and Prettier for code quality and consistent formatting.
3. **Error Handling:**
   - Incorporate structured error handling.
4. **Type Safety:**
   - Adopt TypeScript to reduce runtime errors.

By adhering to these guidelines and executing the specified commands, you can ensure your contributions align with the repository's standards.