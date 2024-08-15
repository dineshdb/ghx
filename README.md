# README

Install binaries from github releases, on-demand.

## How does it work?

We install a shell script at `$GHX_HOME/alias/ghx`. Then we create symbolic
links to it for all the binaries we want it to handle in `$GHX_HOME/alias/*`.
The `ghx` binary will download the required binary on first run of each command
and save it to `$GHX_HOME/bin/<cmd>`. On consecutive runs, the downloaded binary
will be used since it has higher priority than aliases in `$PATH`.

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

# setup $GHX_HOME/alias as fallback. This allows you to override the binaries in other places as well.
# setup $GHX_HOME/bin as overrides. This includes all the downloaded binaries.
export PATH=$GHX_HOME/bin:$PATH:$GHX_HOME/alias
```

## License

MIT

```
```
