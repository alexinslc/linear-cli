# AGENTS.md

## What Is This?
Linear CLI (`lr`) - Go CLI for Linear issue tracker. **WIP - early stage.**

## Quick Facts
- **Tech:** Go + Cobra
- **Purpose:** Manage Linear issues from terminal
- **Status:** Early development

## Key Files
- `main.go` - Entry point
- `cmd/root.go` - Root command

## Commands
```bash
go run main.go  # Run
go build -o lr  # Build
```

## Planned Features
- OAuth login
- Issue CRUD (list, view, create, update, delete)
- Project management
- Local caching

## How to Help
- Follow Cobra patterns (cmd/subcommand)
- Use Linear GraphQL API
- Add commands incrementally
- Include help text for all commands
