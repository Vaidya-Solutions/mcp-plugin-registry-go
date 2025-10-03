# mcp-plugin-registry-go

A tiny, driver-style **builtin plugin registry** for MCP servers (inspired by Go’s `database/sql` pattern).

> **Status:** Early preview — stable enough for examples and discussion. APIs may evolve.

## Why
Keep plugin **construction** decoupled from **registration** so tools can self-register via `init()` or explicit bootstrap, with thread-safe lookups and simple metadata.

## Features (initial)
- Global, thread-safe registry
- Register **factories** (not instances)
- Basic tool metadata & health status hooks
- Zero third-party deps (stdlib only)

## Example (coming soon)
Short snippet and an `examples/` folder will show:
- Registering an `echo` tool
- Listing tools and fetching by name
- Health status checks

## Roadmap
- Optional namespacing
- Init ordering & dependency hints
- Pluggable health reporters

## Contributing
Issues and PRs welcome once the API lands. For now, feel free to open an issue with use-cases.

## License
Apache-2.0 © Vaidya Solutions
