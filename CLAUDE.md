### 🔄 Project Awareness & Context
- **Always read `PLANNING.md`** at the start of a new conversation to understand the project's architecture, goals, style, and constraints.
- **Check `TASK.md`** before starting a new task. If the task isn't listed, add it with a brief description and today's date.
- **Use consistent naming conventions, file structure, and architecture patterns** as described in `PLANNING.md`.
- **Follow the project's established development environment setup** and tooling configurations.

### 🧱 Code Structure & Modularity
- **Never create a file longer than 500 lines of code.** If a file approaches this limit, refactor by splitting it into modules or helper files.
- **Organize code into clearly separated modules**, grouped by feature or responsibility.
  For web components:
    - Keep components focused and single-purpose
    - Separate business logic from presentation
    - Create reusable utility functions
- **Use clear, consistent imports** following the project's module system.
- **Use environment variables** for configuration and sensitive data.

### 🧪 Testing & Reliability
- **Always create unit tests for new features** (functions, components, APIs, etc).
- **After updating any logic**, check whether existing tests need to be updated. If so, do it.
- **Tests should live in a `/tests` or `__tests__` folder** mirroring the main app structure.
  - Include at least:
    - 1 test for expected use
    - 1 edge case
    - 1 failure case

### ✅ Task Completion
- **Mark completed tasks in `TASK.md`** immediately after finishing them.
- Add new sub-tasks or TODOs discovered during development to `TASK.md` under a "Discovered During Work" section.

### 📎 Style & Conventions
- **Follow the project's established coding standards** and linting rules.
- **Use consistent code formatting** with appropriate tools (Prettier, ESLint, etc).
- **Implement proper data validation** for all user inputs and API responses.
- **Use TypeScript** for type safety when applicable.
- Write **clear documentation for functions and complex logic**:
  ```javascript
  /**
   * Brief summary of the function
   * @param {Type} paramName - Description
   * @returns {Type} Description
   */
  ```

### 📚 Documentation & Explainability
- **Update `README.md`** when new features are added, dependencies change, or setup steps are modified.
- **Comment non-obvious code** and ensure everything is understandable to a mid-level developer.
- When writing complex logic, **add inline comments** explaining the why, not just the what.

### 🧠 AI Behavior Rules
- **Never assume missing context. Ask questions if uncertain.**
- **Never hallucinate libraries or functions** – only use known, verified packages from the project's package manager.
- **Always confirm file paths and module names** exist before referencing them in code or tests.
- **Never delete or overwrite existing code** unless explicitly instructed to or if part of a task from `TASK.md`.