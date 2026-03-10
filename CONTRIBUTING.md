# Contributing to open-pi

open-pi is a community-maintained fork of pi-mono. Everyone is welcome here.

## The One Rule

**You must understand your code.** If you can't explain what your changes do and why, your PR will be reviewed carefully — but not auto-closed.

Using AI to write code is fine. AI-assisted contributions are welcome as long as the fix is real, the reasoning is sound, and you can stand behind it.

## First-Time Contributors

1. Open an issue describing what you want to change and why
2. Submit your PR — no approval gate required
5. Once approved, you can submit PRs

This exists because AI makes it trivial to generate plausible-looking but low-quality contributions. The issue step lets us filter early.

## Before Submitting a PR

```bash
npm run check  # must pass with no errors
./test.sh      # must pass
```

Do not edit `CHANGELOG.md`. Changelog entries are added by maintainers.

If you're adding a new provider to `packages/ai`, see `AGENTS.md` for required tests.

## Philosophy

pi's core is minimal. If your feature doesn't belong in the core, it should be an extension. PRs that bloat the core will likely be rejected.

## Questions?

Open an issue or ask on [Discord](https://discord.com/invite/nKXTsAcmbT).
