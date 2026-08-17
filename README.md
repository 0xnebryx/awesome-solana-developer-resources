# awesome-solana-developer-resources

> Curated list of practical Solana developer resources. Maintained by someone who actually ships on Solana.

Inclusion criteria: must be actively maintained, must work in production, must save you time vs rolling your own.

---

## RPC providers

| Provider     | Strengths                                              | Notes                                          |
|--------------|--------------------------------------------------------|------------------------------------------------|
| Helius       | Webhooks, parsed transactions, fast websocket, DAS API | Best DX for non-trivial work                   |
| Triton One   | Dedicated infrastructure, geographically diverse       | Higher-end pricing                             |
| QuickNode    | Multi-chain, good docs, free tier OK for dev           | Latency varies by region                       |
| Alchemy      | Reliable, dashboards, simulation API                   | Solana support newer than EVM                  |
| GenesysGo    | Solana-native, geyser plugins, validator-grade         | Less polished frontend                         |
| Ankr         | Affordable, decent for read-heavy workloads            | Premium tier needed for production             |

## SDKs and core libraries

- [`@solana/web3.js`](https://github.com/solana-labs/solana-web3.js) — official JS client, ubiquitous
- [`@coral-xyz/anchor`](https://github.com/coral-xyz/anchor) — Anchor framework for Rust programs + TS client
- [`@solana/spl-token`](https://github.com/solana-labs/solana-program-library) — SPL token instructions
- [`@solana/spl-token-2022`](https://spl.solana.com/token-2022) — Token-2022 extension support
- [`@nirholas/pump-sdk`](https://www.npmjs.com/package/@nirholas/pump-sdk) — pump.fun bonding curve interactions
- [`@meteora-ag/dlmm`](https://github.com/MeteoraAg/dlmm-sdk) — Dynamic liquidity market makers
- [`@jup-ag/api`](https://station.jup.ag/docs/apis/swap-api) — Jupiter v6 swap API
- [`jito-ts`](https://github.com/jito-labs/mev-protect-sdk) — Jito bundle submission
- [`@sodax/sdk`](https://github.com/icon-project/sodax-sdks) — cross-network execution SDK (swaps, money-market lending, bridging from a Solana wallet across 10+ chains without maintaining bridge infra)

## Frameworks for on-chain programs

- [Anchor](https://www.anchor-lang.com/) — declarative Rust framework, the default choice
- [Native Solana programs](https://solana.com/docs/programs/lang-rust) — direct Rust, more control, more boilerplate
- [Steel](https://github.com/regolith-labs/steel) — minimal alternative to Anchor

## Testing

- [`bankrun`](https://github.com/kevinheavey/solana-bankrun) — fast local test runtime (no validator startup)
- [`solana-test-validator`](https://docs.solana.com/developing/test-validator) — full validator for integration tests
- [Anchor's `mocha` integration](https://www.anchor-lang.com/docs/testing) — TypeScript test runner

## Indexers and data

- [Helius DAS API](https://docs.helius.dev/compression-and-das-api/digital-asset-standard-das-api) — NFT/cNFT metadata
- [Triton Yellowstone gRPC](https://github.com/rpcpool/yellowstone-grpc) — geyser plugin streaming
- [Solana FM](https://solana.fm/) — explorer with pretty TX parsing
- [Solscan](https://solscan.io/) — explorer + analytics
- [Birdeye](https://birdeye.so/) — token + market data API

## Security

- [Neodyme audit checklist](https://github.com/neodyme-labs/solana-security-txt) — security.txt for Solana programs
- [Sec3 auto-auditor](https://www.sec3.dev/) — automated vulnerability scanner
- [Soteria](https://github.com/soteria-dev/soteria) — static analyzer
- [`gitleaks`](https://github.com/gitleaks/gitleaks) — secret scanning (not Solana-specific but mandatory)

## Tooling

- [Solana Playground](https://beta.solpg.io/) — browser-based Anchor/Rust editor + deploy
- [Solana Verify](https://github.com/Ellipsis-Labs/solana-verifiable-build) — reproducible builds for deployed programs
- [Squads multi-sig](https://squads.so/) — multi-sig for treasury management

## Marketplaces and venues

- [pump.fun](https://pump.fun) — bonding curve token launches
- [PumpSwap (Raydium)](https://raydium.io/) — post-graduation AMM
- [Orca](https://www.orca.so/) — concentrated liquidity AMM
- [Meteora](https://meteora.ag/) — dynamic liquidity DLMM
- [Phoenix](https://www.phoenix.trade/) — fully on-chain CLOB

## Learning

- [Solana Cookbook](https://solanacookbook.com/)
- [Solana Course (Soldev)](https://www.soldev.app/course)
- [Anchor Book](https://book.anchor-lang.com/)
- [Solana Bytes (YouTube)](https://www.youtube.com/@SolanaFoundation)

## Communities

- [Solana Stack Exchange](https://solana.stackexchange.com/)
- [Solana Tech Discord](https://discord.com/invite/solana)
- [r/solana](https://reddit.com/r/solana)

---

## Contributing

PRs welcome for tools that meet the inclusion criteria. Mark broken / unmaintained entries via issue. Don't include your own product unless it's a clear win over alternatives.

## License

MIT
