# Copilot Instructions

## Project Overview
Linear CLI (`lr`) - A Go CLI for interacting with Linear issue tracker. Currently a work in progress.

## Tech Stack
- Go 1.21+
- Cobra (CLI framework)

## Structure
- `main.go` - Entry point
- `cmd/` - Cobra commands
  - `root.go` - Root command setup
- `go.mod` / `go.sum` - Dependencies

## Planned Commands
- `lr auth login` - OAuth login
- `lr issue list/view/create/update/delete` - Issue management
- `lr project list/create/update/delete` - Project management
- `lr cache clear/show/update` - Cache management

## Commands
```bash
go run main.go    # Run CLI
go build -o lr    # Build binary
```

## Guidelines
- Follow Cobra patterns for command structure
- Use Linear GraphQL API
- Implement OAuth flow for auth
- Cache data locally for performance
