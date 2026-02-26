# AGENTS.md

## Cursor Cloud specific instructions

This is a static HTML/CSS learning portfolio with no backend or database. Dev tooling is managed via npm.

### Services

| Service | How to run | Notes |
|---|---|---|
| Static file server | `npx http-server -p 8080 -c-1` | Serves all project directories; open `http://localhost:8080` in a browser |

### Key commands

See `package.json` `scripts` for the full list. Summary:

- **Lint (format check):** `npm run format:check` — runs Prettier in check mode. Exits non-zero if files are unformatted (this is expected in the current repo state).
- **Auto-format:** `npm run format` — rewrites files with Prettier.
- **Sass build:** `npm run sass:7` — compiles SCSS to CSS for project 7.
- **Sass watch:** `npm run sass:7:watch` — watches SCSS changes for project 7 (long-running).

### Gotchas

- There are no automated test suites in this repo. Verification is done via `format:check`, `sass:7` compilation, and visual inspection in a browser.
- `npm run format:check` currently exits with code 1 due to pre-existing formatting differences — this is not a bug in your changes.
