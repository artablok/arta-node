# arta-node

Core node implementation for the Arta Blockchain network.

## Status

🚧 **In active development.** This repository currently contains architecture and design documentation.
Source code for the node client will be published here incrementally as development progresses.

## Planned Architecture

The Arta node is designed around the following components:

| Component | Responsibility |
|---|---|
| P2P layer | Peer discovery, block/transaction propagation |
| Consensus module | Block validation and finality |
| State database | Account balances, contract state |
| RPC/API server | JSON-RPC interface for wallets and dApps |
| Smart contract runtime | Execution environment compatible with [arta-contracts](https://github.com/artablok/arta-contracts) |

See [`docs/architecture.md`](./docs/architecture.md) for details.

## Related Repositories

- [arta-core](https://github.com/artablok/arta-core) — ecosystem overview and specifications
- [arta-contracts](https://github.com/artablok/arta-contracts) — smart contracts
- [arta-sdk](https://github.com/artablok/arta-sdk) — client SDK

## Contributing

This project is in early-stage development. Issues and design discussions are welcome via the
[Issues](https://github.com/artablok/arta-node/issues) tab.

## License

MIT
