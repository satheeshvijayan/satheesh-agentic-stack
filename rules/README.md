# Rules

## Structure

Rules are organized into a **common** layer plus **language-specific** directories:

```
rules/
├── common/          # Language-agnostic principles (always install)
│   ├── coding-style.md
│   ├── git-workflow.md
│   ├── testing.md
│   ├── performance.md
│   ├── patterns.md
│   ├── hooks.md
│   ├── agents.md
│   └── security.md
├── python/          # Python specific
└── typescript/      # TypeScript/JavaScript specific
```

## Installation

> **Note:** Rules must be manually copied to `~/.claude/rules/` — they are not auto-loaded by the plugin system.

```bash
# Install common rules (required)
cp -r rules/common ~/.claude/rules/common

# Install Python rules
cp -r rules/python ~/.claude/rules/python

# Install TypeScript rules
cp -r rules/typescript ~/.claude/rules/typescript
```

> **Important:** Copy entire directories — do NOT flatten with `/*`.
> Common and language-specific directories contain files with the same names.
> Flattening causes language-specific files to overwrite common rules.

## Rule Priority

When language-specific rules and common rules conflict, **language-specific rules take precedence**.
