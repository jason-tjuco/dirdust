# dirdust

Small Go tool: declutter ~/Downloads in one command

Built for my own use; public in case it helps someone.

## Features

- Groups files into folders by extension
- Skips hidden files and folders by default
- Single static binary, no runtime deps
- Dry-run prints the plan before moving anything

## How to use

```bash
./bin/dirdust ~/Downloads --dry-run
./bin/dirdust ~/Downloads
```

## Getting started

```bash
go build -o bin/ ./...
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── LICENSE
├── SECURITY.md
├── go.mod
└── main.go
```

## Development

```bash
go build ./...
go vet ./...
```

## Changelog

- `0.1.1` - fix edge case in argument parsing
- `0.1.0` - first working version

## License

MIT. Do whatever you want.
