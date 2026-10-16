# Welcome to swe-kda-community

Kadena AI ecosystem tools and releases.

## What We Build

AI-focused development (community-based effort) for the Kadena Chainweb blockchain.

## Repositories of Interest

- [`kda-branch-kadena.js`](https://github.com/swe-kda-community/kda-branch-kadena.js) — Workspaces for kadena.js sections
- [`kda-branch-pact-5-post_quantum`](https://github.com/swe-kda-community/kda-branch-pact-5-post_quantum) — Workspace for post_quantum work on pact-5

## In Development

Sneak preview — what we're working on next:

- `swe-pact-contracts` — pact contracts for testing and to build against !!

## Download Builds

Binaries for all projects: **https://github.com/swe-kda-community/releases**

### Homebrew

```bash
brew trust swe-kda-community/tap
brew tap swe-kda-community/tap
brew install <formula>
```

## Getting Help

Open an issue in the relevant repository.

## For Developers: Bootstrap Your Own Org

Running your own org and want the same structure? The tool we use to set this up lives in our shared tooling org:

**[homebrew-tap-app](https://github.com/kore-kda-community/homebrew-tap-app)** — a single script that scaffolds:

- **`.github`** — org profile README + shared community health files
- **`releases`** — central hub where every tagged build lands
- **`homebrew-tap`** — package manager formulae, auto-bumped by CI
- **Source repos** — one per project, with branch layout for project work
- **Release workflow** — GoReleaser config + GitHub Actions; tag → build → publish → formula bump, fully automated
- **Release schedule** — driven by tags, so `git tag vX.Y.Z && git push --tags` is the whole workflow

Clone it, point it at your org, run `./run.sh`. Safe to re-run.