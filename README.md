# neoswarm/homebrew-tap

Homebrew formulae for [neosh](https://github.com/neoswarm/neosh) — a terminal-first agent
workspace where every feature is a plugin.

```sh
brew install neoswarm/tap/neosh
```

Or tap it once and use the bare name afterwards:

```sh
brew tap neoswarm/tap
brew install neosh
```

macOS and Linux, on both Apple silicon / ARM64 and x86-64. The formula installs a prebuilt binary
from the [neosh releases](https://github.com/neoswarm/neosh/releases) — no Rust toolchain and no
quarter-hour build.

## Why a tap rather than homebrew-core

homebrew-core has notability requirements a young project does not meet, and a tap has none while
being the same one line to whoever is typing it. Core is worth revisiting later; nothing about the
formula would change.

## Updating

`Formula/neosh.rb` is generated, never hand-edited — the checksums come from the release itself:

```sh
# in a neosh checkout, once the release workflow has finished
scripts/brew-formula.sh v0.1.0 > /path/to/homebrew-tap/Formula/neosh.rb
```
