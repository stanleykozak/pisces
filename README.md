## match-pair fish plugin

[![](https://img.shields.io/badge/fish--shell-2.3b2-blue.svg)](https://github.com/fish-shell/fish-shell/releases/tag/2.3b2)
[![](https://img.shields.io/badge/license-LGPLv3-blue.svg)](https://www.tldrlegal.com/l/lgpl-3.0)
[![](https://img.shields.io/badge/contact-gitter_chat-dd1054.svg)](https://gitter.im/laughedelic/match-pair.fish)

This plugin handles matching pair symbols like `''`, `""`, `()`, `[]` and `{}` in your fish command line. Just like you favorite text editor!

### Features

Here `|` denotes the current cursor position. No manual cursor motion involved :sparkles:

- [x] autocloses pair symbol: `... |` + `(` => `... (|)`
- [x] skips the closing symbol: `... |)` + `)` => `... )|`
- [x] removes empty pairs: `...(|)` + `backspace` => `...`
- [ ] doesn't autoclose escaped symbols: `...\|` + `(` => `...\(|`
- [x] configurable set of symbol pairs: `set -U match_pairs '< >' $match_pairs`
- [ ] conditional autoclosing (don't autoclose if the cursor is on certain symbols)


### Installation

With [fisherman](https://github.com/fisherman/fisherman):

```fish
fisherman install laughedelic/match-pair.fish
```
