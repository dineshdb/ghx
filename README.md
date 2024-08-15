# README

Install binaries from github releases, on-demand.

## Setup

- Download this repo.
- Run `bin/ghx`.
- Add following to your `.profile`

```
export GHX_HOME=$HOME/.local/ghx
# setup $GHX_HOME/alias as fallback. This allows you to override the binaries in other places.
# setup $GHX_HOME/bin as overrides. This includes all the downloaded binaries.
export PATH=$GHX_HOME/bin:$PATH:$GHX_HOME/alias
```

## Features

- [x] Download the aliasmap from github url
- [ ] Remove need to download/clone the repo to setup.
- [ ] One line setup.

## License

MIT
