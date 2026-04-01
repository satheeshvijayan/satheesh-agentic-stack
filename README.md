# satheesh-agentic-stack

A curated Claude Code plugin optimized for **Python, Django, FastAPI, PostgreSQL, MongoDB, React, gRPC, microservices, and Agentic AI workflows**.

Built from a selective curation of [everything-claude-code](https://github.com/affaan-m/everything-claude-code), keeping only what matters for modern backend and AI-first development.

## Tech Stack Coverage

- **Backend**: Python, Django, FastAPI
- **Databases**: PostgreSQL, MongoDB
- **Frontend**: React, TypeScript
- **Infrastructure**: Docker, gRPC, microservices
- **AI/ML**: Agentic AI loops, LLM pipelines, RAG, evaluation harnesses

## Components

### Agents (12)

| Agent | Purpose |
|-------|---------|
| `planner` | Task decomposition and implementation planning |
| `architect` | System design and architecture decisions |
| `tdd-guide` | Test-driven development workflow |
| `code-reviewer` | General code review |
| `security-reviewer` | Security-focused review |
| `python-reviewer` | Python-specific review |
| `database-reviewer` | Database schema and query review |
| `typescript-reviewer` | TypeScript/React review |
| `build-error-resolver` | Build and compilation error fixing |
| `refactor-cleaner` | Code refactoring and cleanup |
| `doc-updater` | Documentation maintenance |
| `loop-operator` | Autonomous loop orchestration |

### Skills (21)

**Core Stack:**
`backend-patterns` `api-design` `django-patterns` `django-security` `django-tdd` `python-patterns` `python-testing` `database-migrations` `postgres-patterns` `docker-patterns` `deployment-patterns` `e2e-testing` `frontend-patterns`

**Agentic AI / Advanced:**
`cost-aware-llm-pipeline` `iterative-retrieval` `verification-loop` `autonomous-loops`

**Quality & Security:**
`search-first` `eval-harness` `security-review` `continuous-learning-v2`

### Commands (9)

| Command | Purpose |
|---------|---------|
| `/plan` | Create implementation plans |
| `/tdd` | Run TDD workflow |
| `/code-review` | Trigger code review |
| `/build-fix` | Fix build errors |
| `/refactor-clean` | Refactor and clean code |
| `/verify` | Verify implementation |
| `/multi-plan` | Multi-service planning |
| `/multi-execute` | Multi-service execution |
| `/orchestrate` | Full orchestration workflow |

### Rules (3 directories)

- `common/` — Language-agnostic coding standards (10 files)
- `python/` — Python-specific rules (5 files)
- `typescript/` — TypeScript-specific rules (5 files)

> **Note:** Rules require manual installation to `~/.claude/rules/`. See `rules/README.md`.

### Contexts (3)

- `dev.md` — Development context
- `review.md` — Code review context
- `research.md` — Research context

### Hooks

- `hooks.json` — Pre/post tool execution hooks

## Installation

### From GitHub (Marketplace)

```bash
# Add the marketplace
/plugin marketplace add satheeshvijayan/satheesh-agentic-stack

# Install the plugin
/plugin install satheesh-agentic-stack@satheesh-marketplace
```

### Manual Installation

```bash
git clone https://github.com/satheeshvijayan/satheesh-agentic-stack.git
cd satheesh-agentic-stack

# Copy rules manually (required — not auto-loaded by plugin system)
cp -r rules/common ~/.claude/rules/common
cp -r rules/python ~/.claude/rules/python
cp -r rules/typescript ~/.claude/rules/typescript
```

## Usage

Once installed, agents, skills, and commands are available in Claude Code:

```bash
# Use a command
/plan "Add user authentication to the API"

# Run TDD workflow
/tdd "Implement the payment service"

# Orchestrate a multi-service task
/orchestrate "Deploy the new microservice"
```

## Credits

This plugin is a curated subset of [everything-claude-code](https://github.com/affaan-m/everything-claude-code) by [affaan-m](https://github.com/affaan-m). Full credit to the original authors for the comprehensive agent, skill, and rule definitions.

## License

MIT
