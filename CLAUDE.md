# Project Rules & Guidelines

## =« ABSOLUTE RULES - NEVER VIOLATE

### NEVER DO:
- **NEVER use emojis** in code, comments, commits, or any technical documentation
- **NEVER create files longer than 500 lines** - split into modules immediately
- **NEVER assume or hallucinate libraries** - verify all packages exist first
- **NEVER delete existing code** without explicit user instruction
- **NEVER create documentation files** unless explicitly requested (no README, no docs)
- **NEVER commit to git** unless explicitly asked by the user
- **NEVER push to remote** unless explicitly instructed
- **NEVER modify git config** or user settings
- **NEVER expose sensitive data** like API keys, passwords, or tokens
- **NEVER skip tests** when implementing features
- **NEVER ignore error handling** - all errors must be caught and handled

### ALWAYS DO:
- **ALWAYS read PLANNING.md** at conversation start for project context
- **ALWAYS check TASK.md** before starting new work
- **ALWAYS prefer editing existing files** over creating new ones
- **ALWAYS verify file paths exist** before referencing them
- **ALWAYS use environment variables** for configuration
- **ALWAYS write tests** for new features (minimum 3: happy path, edge case, failure)
- **ALWAYS follow existing code patterns** in the project
- **ALWAYS ask for clarification** when requirements are unclear
- **ALWAYS validate user inputs** and API responses
- **ALWAYS handle errors gracefully** with user-friendly messages

## =Ë Development Standards

### Code Organization
- **Maximum file size**: 500 lines (refactor if approaching limit)
- **Module structure**: Feature-based organization
- **Import style**: Use consistent import patterns (relative within packages)
- **Naming conventions**: Follow project's established patterns
- **Component focus**: Single responsibility principle

### Testing Requirements
- **Test location**: `/tests` or `__tests__` directories
- **Test coverage**: Minimum 80% for new code
- **Test types required**:
  - Unit tests for all functions/components
  - Integration tests for APIs
  - E2E tests for critical user paths
- **Test before commit**: All tests must pass

### Code Quality
- **Linting**: Follow project's ESLint/Prettier configuration
- **Type safety**: Use TypeScript when available
- **Comments**: Only for complex logic (explain why, not what)
- **Documentation**: JSDoc for public APIs
- **Error handling**: Try-catch blocks, error boundaries
- **Performance**: Optimize for Core Web Vitals

### Security & Best Practices
- **Input validation**: Sanitize all user inputs
- **API security**: Use HTTPS, implement CORS properly
- **Authentication**: Secure session management
- **Dependencies**: Keep updated, audit regularly
- **Secrets management**: Use environment variables only
- **Data protection**: Follow GDPR/privacy requirements

## <¯ Project Initialization Checklist

When starting a new project with this template:

1. **Define project type** in INITIAL.md:
   - Web application (React/Vue/Angular/etc.)
   - API service (REST/GraphQL)
   - Full-stack application
   - Library/Package
   - CLI tool

2. **Specify technical stack**:
   - Framework choice
   - Database requirements
   - Authentication needs
   - Deployment target

3. **Set project constraints**:
   - Performance requirements
   - Browser support
   - Mobile responsiveness
   - Accessibility standards

4. **Provide examples** in `/examples` folder:
   - Code patterns to follow
   - Component structures
   - API implementations
   - Test patterns

## = Workflow Rules

### Before Starting Work
1. Read project context (PLANNING.md)
2. Check current tasks (TASK.md)
3. Understand existing patterns (examples/)
4. Verify development environment

### During Development
1. Follow TDD approach when applicable
2. Keep commits atomic and focused
3. Update tests for modified code
4. Maintain consistent code style
5. Document breaking changes

### After Completing Features
1. Run all tests
2. Verify linting passes
3. Update TASK.md
4. Check for performance impacts
5. Ensure accessibility compliance

## =€ Quick Start Commands

```bash
# Initialize new project from this template
/initialize-project

# Generate implementation plan
/generate-prp INITIAL.md

# Execute implementation
/execute-prp PRPs/[feature-name].md

# Run tests
npm test / yarn test / pnpm test

# Check code quality
npm run lint / yarn lint / pnpm lint
```

## =Ý Task Management

### Task Tracking
- Mark tasks in TASK.md immediately upon completion
- Add discovered subtasks during development
- Keep task descriptions clear and actionable
- Include acceptance criteria for complex tasks

### Progress Reporting
- Use clear status indicators (pending/in-progress/completed)
- Document blockers immediately
- Update estimates when scope changes
- Communicate assumptions made

## ™ Environment Setup

### Required Tools
- Node.js (LTS version)
- Package manager (npm/yarn/pnpm)
- Git for version control
- Code editor with project config support

### Configuration Files
- `.env` for environment variables
- `.gitignore` for excluded files
- `package.json` for dependencies
- Config files for tools (ESLint, Prettier, etc.)

## <¨ UI/UX Guidelines

### Design Principles
- Mobile-first responsive design
- Accessibility (WCAG 2.1 AA minimum)
- Consistent visual hierarchy
- Clear navigation patterns
- Appropriate loading states

### Performance Targets
- Lighthouse score > 90 all categories
- First Contentful Paint < 1.8s
- Time to Interactive < 3.8s
- Cumulative Layout Shift < 0.1

## =Ê Monitoring & Maintenance

### Code Health
- Regular dependency updates
- Security audit schedule
- Performance monitoring
- Error tracking setup
- Analytics implementation

### Documentation Updates
- Keep README current
- Update API documentation
- Maintain changelog
- Document deployment process
- Record architecture decisions

---

**Remember**: This file defines the rules for AI assistants working on this project. Follow these guidelines strictly to ensure consistent, high-quality code delivery.