# README

Install binaries from github releases, on-demand.

## Setup

### automatic path setup

```
curl -sSf https://raw.githubusercontent.com/dineshdb/ghx/main/bin/install | bash \
-s -- --setup-path
```

### with manual path setup

```
curl -sSf https://raw.githubusercontent.com/dineshdb/ghx/main/bin/install | bash
```

### Manual path setup

```
export GHX_HOME=$HOME/.local/ghx

# setup $GHX_HOME/alias as fallback. This allows you to override the binaries in other places.

# setup $GHX_HOME/bin as overrides. This includes all the downloaded binaries.

export PATH=$GHX_HOME/bin:$PATH:$GHX_HOME/alias
```

## License

MIT

```
```
