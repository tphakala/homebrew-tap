# tphakala/homebrew-tap

A [Homebrew](https://brew.sh) tap for my tools.

## Install

```sh
brew tap tphakala/tap
brew install agy-mcp
```

Or in one line without tapping first:

```sh
brew install tphakala/tap/agy-mcp
```

Upgrade later with `brew upgrade agy-mcp`, remove with `brew uninstall agy-mcp`.

## Formulae

| Formula | Description |
| --- | --- |
| [`agy-mcp`](Formula/agy-mcp.rb) | MCP server for the Google Antigravity CLI (`agy`) with async supervision and completion wakes. See [tphakala/agy-mcp](https://github.com/tphakala/agy-mcp). |

Formulae install the prebuilt release binaries published to each project's GitHub releases (macOS and Linux, amd64 and arm64). No bottles are published.

## How this tap stays current

Formulae here are updated automatically, never by hand. Each source project builds its release with [GoReleaser](https://goreleaser.com), and its `brews` configuration regenerates the formula in this repo and commits it on every tagged release. A push here therefore lands within seconds of the upstream release, with the new version and the SHA-256 of every archive already filled in.

CI pushes are authorized with a per-repo deploy key that has write access to this tap only, so no personal access token is involved and the blast radius is limited to this one repository.

The `Formula/*.rb` files are generated. Do not edit them directly; change the source project's GoReleaser config instead.

## License

The tap metadata is MIT licensed. Each installed tool carries its own license.
