<p align="center">
  <a href="https://github.com/FuzzyFade/open-pi">
    <img src="./logo.svg" alt="open-pi logo" width="128">
  </a>
</p>
<p align="center">
  <a href="https://github.com/FuzzyFade/open-pi/actions/workflows/ci.yml"><img alt="Build status" src="https://img.shields.io/github/actions/workflow/status/FuzzyFade/open-pi/ci.yml?style=flat-square&branch=main" /></a>
</p>

# open-pi

> **The open AI agent toolkit. No gatekeeping.**

A community-maintained fork of [pi-mono](https://github.com/FuzzyFade/open-pi) — open to all contributors, including AI-assisted ones. We judge contributions by their quality, not their origin.

> **Looking for the coding agent?** See **[packages/coding-agent](packages/coding-agent)** for installation and usage.

Tools for building AI agents and managing LLM deployments.

## Packages

| Package | Description |
|---------|-------------|
| **[open-pi-ai](packages/ai)** | Unified multi-provider LLM API (OpenAI, Anthropic, Google, etc.) |
| **[open-pi-agent](packages/agent)** | Agent runtime with tool calling and state management |
| **[open-pi-coding-agent](packages/coding-agent)** | Interactive coding agent CLI |
| **[open-pi-mom](packages/mom)** | Slack bot that delegates messages to the pi coding agent |
| **[open-pi-tui](packages/tui)** | Terminal UI library with differential rendering |
| **[open-pi-web-ui](packages/web-ui)** | Web components for AI chat interfaces |
| **[open-pi-pods](packages/pods)** | CLI for managing vLLM deployments on GPU pods |

## Contributing

We welcome contributions from everyone — human or AI-assisted. If your fix is real and your reasoning is sound, it belongs here.

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines and [AGENTS.md](AGENTS.md) for project-specific rules.

## Development

```bash
npm install          # Install all dependencies
npm run build        # Build all packages
npm run check        # Lint, format, and type check
./test.sh            # Run tests (skips LLM-dependent tests without API keys)
./pi-test.sh         # Run pi from sources (must be run from repo root)
```

> **Note:** `npm run check` requires `npm run build` to be run first. The web-ui package uses `tsc` which needs compiled `.d.ts` files from dependencies.

## License

MIT
