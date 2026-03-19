# nix-statix-bin

Prebuilt [statix](https://github.com/nerdypepper/statix) binaries for nix anti-pattern linting.

## Install via mise

```toml
[tools]
"github:prettygood-software/nix-statix-bin" = "latest"
```

## Platforms

| Target | Runner |
|--------|--------|
| `aarch64-apple-darwin` | macOS 14 (Apple Silicon) |
| `x86_64-unknown-linux-gnu` | Ubuntu latest |
| `aarch64-unknown-linux-gnu` | Ubuntu latest (cross) |

## Updating

Run the **Build and Release** workflow with the upstream version (e.g. `0.5.8`).

The **Check Upstream Release** workflow runs weekly and creates an issue when a new version is available.

## Development

Prerequisites: [mise](https://mise.jdx.dev/)

```bash
# Install tools and git hooks
task setup

# Run all linters (actionlint + yamllint + tool.json validation)
task lint
```
