# ChainSight — AI Blockchain Forensics

> See through the chain. AI-powered fund tracing, pattern detection, and compliance reporting.
> **MiMo V2.5** powers the forensic brain. **Hermes Agent** powers the runtime.

## What is ChainSight?

ChainSight is an AI-powered blockchain forensics engine that lets investigators trace fund flows, detect suspicious patterns, and generate compliance-grade reports through natural language queries.

### Core Capabilities

- **Trace** — Follow funds across chains, bridges, mixers, and DEXs. Multi-hop path reconstruction with automatic entity labeling.
- **Detect** — Real-time anomaly detection: wash trading, sandwich attacks, rug pulls, flash loan exploits.
- **Report** — Generate compliance-grade investigation reports in natural language. Timeline reconstruction, risk scoring, evidence chain.

### Architecture

```
Data Sources → MiMo V2.5 (Reasoning) → Outputs
  EVM RPC/8 chains     NL → Investigation plan    PDF/Markdown reports
  Bridges (Across,     Pattern match + Risk score  Real-time alerts
    Stargate, etc)     Entity resolution           REST API
  Mixers (Tornado,     Multi-hop trace reasoning   Webhook delivery
    FixedFloat, etc)
```

### Risk Classification

| Level | Description | Scope |
|---|---|---|
| CRITICAL | Confirmed exploit/hack/sanctioned entity | 142 addresses |
| HIGH | Strong indicators: mixer usage, fresh wallet patterns | 1,847 addresses |
| MEDIUM | Unusual activity: high-freq trades, dust attacks | 12,403 addresses |
| LOW | Clean with verifiable history | 2.1M addresses |

## Stack

| Component | Technology |
|---|---|
| **Runtime** | Hermes Agent v0.14.0 (self-hosted) |
| **Reasoning** | MiMo V2.5 (Xiaomi MiMo Open Platform) |
| **Agent Framework** | SOUL.md constitution + AGENTS.md router |
| **Skills** | 100+ procedural playbooks (crypto, forensics, automation) |
| **Chains** | Ethereum, Base, Arbitrum, Optimism, Polygon, BSC, Sepolia, Base Sepolia |

## Live Demo

🌐 **[chainsight-landing](https://chainsight.vercel.app/)** — Interactive landing page with animated fund flow visualization

## Proof of Operation

| Artifact | Link |
|---|---|
| Source Repository | [github.com/santuy69/chainsight-landing](https://github.com/santuy69/chainsight-landing) |
| Agent Wallet | [0xc086…A064c](https://etherscan.io/address/0xc086A8aacB0BD742c9E7C3499E07e651298A064c) |
| Runtime Evidence | [proof/](https://github.com/santuy69/chainsight-landing/tree/main/proof) |
| X / Twitter | [@0x_Missy22](https://x.com/0x_Missy22) |

## Why MiMo V2.5?

1. **Multi-hop trace reasoning** — Following funds through 6+ hops requires consistent context retention
2. **Real-time alert speed** — Sub-5-second analysis before funds disappear into mixers
3. **Structured report generation** — Precise language, accurate numbers, verifiable evidence chains

## License

MIT — see [LICENSE](LICENSE)

---

*Built with Hermes Agent + MiMo V2.5 · 2026*
