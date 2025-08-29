# Initialize Project Command

## Description
Interactive command to help fill out the CLAUDE.md and INITIAL.md template files by asking targeted questions about your project requirements. This prepares your project for the PRP generation and execution workflow.

## Usage
```bash
/initialize-project
```

## Implementation

I'll help you initialize your project by asking targeted questions to fill out the CLAUDE.md and INITIAL.md templates. This sets you up for the workflow:
1. `/initialize-project` (fill templates)
2. `/generate-prp INITIAL.md` (create implementation plan)
3. `/execute-prp PRPs/[feature-name].md` (build the project)

Let me ask you some questions to customize your project templates:

### Step 1: Basic Project Information

**Question 1**: What's your project name?

**Question 2**: What type of project are you building?
- Web Application (React/Vue/Angular/Svelte)
- API Service (REST/GraphQL)
- Full-stack Application
- Library/Package
- CLI Tool
- Mobile App (React Native/Flutter)
- Desktop App (Electron/Tauri)
- Other

**Question 3**: In one sentence, what does this project do and why does it exist?

### Step 2: Technical Stack Preferences

**Question 4**: What's your preferred frontend framework? (if applicable)
- React
- Vue.js
- Angular
- Svelte
- Vanilla JavaScript
- Other/None

**Question 5**: What's your preferred backend technology? (if applicable)
- Node.js (Express/Fastify/NestJS)
- Python (FastAPI/Django/Flask)
- Go
- Rust
- Java/Kotlin
- Other/None

**Question 6**: What's your preferred database?
- PostgreSQL
- MySQL
- MongoDB
- SQLite
- Redis
- None
- Other

**Question 7**: Where do you plan to deploy?
- Vercel
- Netlify
- AWS
- Azure
- GCP
- Self-hosted
- Other

### Step 3: Project Rules & Constraints

**Question 8**: Are there any specific coding rules you want enforced? (e.g., "Never use any", "Always use async/await", "Must have 90%+ test coverage")

**Question 9**: What are your performance requirements?
- Basic (no specific requirements)
- High performance (Lighthouse > 90, fast loading)
- Enterprise scale (handle thousands of users)
- Other specific requirements

**Question 10**: Any specific features or integrations needed?
- Authentication (OAuth, email/password, etc.)
- Payment processing (Stripe, PayPal)
- Real-time features (WebSockets, Server-Sent Events)
- File uploads/storage
- Email sending
- Third-party APIs
- Other

### Step 4: Development Preferences

**Question 11**: What testing approach do you prefer?
- Unit tests only
- Unit + Integration tests
- Unit + Integration + E2E tests
- Minimal testing
- Other

**Question 12**: Any accessibility requirements?
- WCAG 2.1 AA compliance
- Basic accessibility
- No specific requirements
- Other

Based on your answers, I'll:
1. Update INITIAL.md with your specific project requirements
2. Customize CLAUDE.md with your project-specific rules and preferences
3. Set up the template so you can run `/generate-prp INITIAL.md` next

Please answer these questions, and I'll customize your template files accordingly!