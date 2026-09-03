# Node Architecture (Design Draft)

This document describes the planned architecture of the Arta node client. It is a design
reference, not a description of already-implemented functionality — see the main
[README](../README.md) for current status.

## Goals

- Deterministic, auditable state transitions
- Compatibility with existing EVM tooling for smart contract deployment
- Lightweight resource footprint suitable for community-run nodes

## Components

### 1. Networking layer
Handles peer discovery and gossip of blocks and pending transactions between nodes.

### 2. Consensus
Validates incoming blocks against protocol rules and maintains canonical chain state.

### 3. State database
Persists account balances, contract storage, and chain metadata.

### 4. RPC interface
Exposes a JSON-RPC API for wallets, block explorers, and dApp frontends to query chain state
and submit transactions.

## Open Questions

- Final consensus mechanism selection
- State database backend (see [arta-core specs](https://github.com/artablok/arta-core/blob/main/specs/network.md) for related discussion)

Feedback and proposals are tracked via [arta-improvement-proposals](https://github.com/artablok/arta-improvement-proposals).
