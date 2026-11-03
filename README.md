# fastevm-workspace

Workspace tying the fastevm engine to Ethereum execution clients.

| path | repo | branch |
|---|---|---|
| `fastevm/` | [Magicking/evm-opencl](https://github.com/Magicking/evm-opencl) | `main` |
| `besu/` | [Magicking/besu](https://github.com/Magicking/besu) (fork of besu-eth/besu) | `fastevm` |
| `go-ethereum/` | [Magicking/geth](https://github.com/Magicking/geth) (fork of ethereum/go-ethereum) | `fastevm` |
| `reth/` | [Magicking/reth](https://github.com/Magicking/reth) (fork of paradigmxyz/reth) | `fastevm` |

```sh
git clone --recurse-submodules https://github.com/Magicking/fastevm-workspace
# later: git submodule update --remote
```

`go-ethereum` and `reth` reference the engine bindings via relative paths
(`../fastevm/bindings/...`), so keep the directory layout as is.
