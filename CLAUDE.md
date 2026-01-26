# CLAUDE.md

## Project Overview
Linear CLI (`lr`) - A Go CLI for Linear issue tracker. **Work in progress.**

## Tech Stack
- **Language:** Go 1.21+
- **CLI Framework:** Cobra
- **API:** Linear GraphQL API (planned)

## Project Structure
```
linear-cli/
├── main.go       # Entry point
├── cmd/
│   └── root.go   # Root Cobra command
├── go.mod
└── go.sum
```

## Development
```bash
go run main.go      # Run
go build -o lr      # Build binary
./lr --help         # Show help
```

## Planned Features
### Auth
- `lr auth login` - OAuth with Linear

### Issues
- `lr issue list` - List issues
- `lr issue view <id>` - View issue details
- `lr issue create` - Create new issue
- `lr issue update <id>` - Update issue
- `lr issue delete <id>` - Delete issue
- `lr issue comment <id>` - Add comment
- `lr issue assign <id>` - Assign issue

### Projects
- `lr project list/create/update/delete`

### Cache
- `lr cache clear/show/update`

## Implementation Notes
- Uses Cobra for command structure
- Will need Linear API key or OAuth
- Consider caching for performance
- Follow Linear's GraphQL schema

## Resources
- [Linear API Docs](https://developers.linear.app/docs)
- [Cobra Docs](https://cobra.dev/)
