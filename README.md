# foundry-erc20-tutorial

> Learning Solidity + Foundry from scratch — Week 1 of an 8-week Web3 sprint toward a smart contract / AI agent engineer role.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Foundry](https://img.shields.io/badge/Foundry-1.5.1-red.svg)](https://book.getfoundry.sh/)
[![Built with Claude Code](https://img.shields.io/badge/Built%20with-Claude%20Code-D97706.svg)](https://www.anthropic.com/claude-code)

## What · Why · How

- **What** — A hands-on Foundry project where I learn ERC-20/721/4626 standards by implementing them with 100% test coverage, including fuzz and invariant tests.
- **Why** — Transitioning from product to smart contract engineer. This repo is my public learning log + portfolio proof for Web3 job applications (Byterum, Trust Wallet, Bybit Audit Intern, Foresight VC, etc.).
- **How** — Daily commits following the [Cyfrin Updraft Foundry Fundamentals](https://updraft.cyfrin.io/courses/foundry) curriculum, augmented with OpenZeppelin source reading and Damn Vulnerable DeFi challenges.

## Progress

| Milestone | Status | Commit |
|-----------|--------|--------|
| W1 D1 · Foundry environment + first project init | ✅ | [cee14c3](../../commit/cee14c3) |
| W1 D5 · LICENSE + professional README | ✅ | *this one* |
| W1 D5 · First custom test `test_IncrementTwice` | ⏳ | — |
| W1 D6 · ERC-20 from scratch with fuzz tests | ⏳ | — |
| W1 D7 · ERC-721 with royalty (EIP-2981) | ⏳ | — |
| W2 · ERC-4626 vault + invariant tests | ⏳ | — |
| W2 · Security: reentrancy, DVD first 5 levels | ⏳ | — |

## Quick Start

```bash
# Clone
git clone https://github.com/Xiaozhi92/foundry-erc20-tutorial.git
cd foundry-erc20-tutorial

# Install Foundry if you haven't
curl -L https://foundry.paradigm.xyz | bash
foundryup

# Run the test suite
forge test -vv
```

## Project Structure

```
src/                  → Solidity contracts
  Counter.sol         ← starter template
test/                 → Foundry test files (*.t.sol)
  Counter.t.sol       ← unit + fuzz tests
script/               → Deployment scripts
lib/forge-std/        → Foundry's test stdlib
foundry.toml          → Project config
```

## Key Concepts Tracked

Every Solidity / Foundry / DeFi term I encounter gets logged in a living glossary, rated by interview frequency and mastery level. Current coverage (W1 D5): **50 terms** across 10 categories.

## Foundry Commands Cheat Sheet

| Command | Purpose |
|---------|---------|
| `forge build` | Compile contracts |
| `forge test` | Run all tests |
| `forge test -vvv` | Tests with verbose trace |
| `forge test --gas-report` | Tests + gas consumption report |
| `forge coverage` | Test coverage report |
| `forge fmt` | Format `.sol` files |
| `forge snapshot` | Save gas snapshot for comparison |
| `anvil` | Start local Ethereum node (port 8545) |
| `cast call <addr> "fn(types)"` | Read on-chain state |
| `cast send <addr> "fn(types)" args` | Send transaction |

## Documentation

- [Foundry Book](https://book.getfoundry.sh/) — Official Foundry docs
- [Solidity Docs](https://docs.soliditylang.org/) — Solidity language reference
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) — Battle-tested standard implementations

## Author

**Xiaozhi** · [GitHub](https://github.com/Xiaozhi92)

Former product engineer transitioning to smart contract × AI agent engineering. Background: 6.5 years overseas (US 5y + SG 1.5y), Claude-native builder, previously built AI agent products with vector memory systems.

Follow my 8-week sprint publicly — raw, iterative, and transparent.

## License

[MIT](LICENSE) — free to fork, learn, reuse.

---

🤖 **Built with [Claude Code](https://www.anthropic.com/claude-code).** Each commit reflects a real learning milestone.
