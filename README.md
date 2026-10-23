# Eddy Flores — AliceLabs LLC

**Trust infrastructure for AI agents.** Receipts, not vibes.

I build the full stack that answers one question: *should this agent be allowed to do that?* Identity, translation, audit, enforcement — every claim on this page links to a repo, a live receipt or a spec. Nothing here is a vibe.

**Live:** [utalabs.tech](https://utalabs.tech) · [alicelabs.site](https://alicelabs.site) · [marketnow.site](https://marketnow.site)

---

## The utalabs.tech stack

Four files, one question. Each product answers it at a different layer.

| Layer | Product | What it is | Proof |
|---|---|---|---|
| 01 · translation | [**UTA**](https://utalabs.tech/uta/) — universal trust adapter | 8 credential formats in (JWT, W3C VC, A2A, X.509, ATC…), one canonical schema out. 12-stage verification pipeline. | [x402 API](https://uta-trust-api.eddyflores100.workers.dev) — $0.01/verify, fail-closed |
| 02 · identity | [**ATC**](https://utalabs.tech/atc/) — agent trust card | Ed25519-signed capability card (ATC/1.0, RFC v3.0): who the agent is, what it may touch, who answers for it. | 57 cards live · MNR-CRL-1.0 revocation |
| 03 · audit | [**Sentinel**](https://utalabs.tech/sentinel/) | 10 static layers + a real L2 sandbox: every MCP server executed under gVisor, syscalls watched for 30 s. | 1,211,488 checks · 1,030 threats caught |
| 04 · enforcement | [**Interceptor**](https://utalabs.tech/interceptor/) | MCP runtime policy engine. Blocks `.env` reads and `rm -rf` even when the caller's card is valid. | 5 live rules · signed JSONL audit trail |
| annex A · provider side | [**UTA-Shield**](https://wall.utalabs.tech) — firewall for MCP operators | Wraps your MCP server once: identity gates, threat-intel blocking (23 live IOCs from a real takedown), rate limits, DLP, x402 metering. 19.8 kB, zero dependencies. | [repo](https://github.com/eddyflores100-lang/uta-shield) |
| annex B · registry | [**MarketNow**](https://marketnow.site) | Trust registry & marketplace: skills, credentials and domains verified across 68,388 MCP servers indexed. | free MCP API, 9 tools, no signup |

Fail-closed is the house rule: unreachable revocation check → DENY. Downtime degrades to "no", never to "probably fine".

## SLOTH — the overnight agent that hands you a receipt

[**sloth.utalabs.tech**](https://sloth.utalabs.tech) · [repo](https://github.com/eddyflores100-lang/sloth)

**S**leepy **L**azy **O**vernight **T**ask **H**andler. A 1B open-weight brain (Gemma 3 + llama.cpp) that runs on your CPU and does the boring stuff while you sleep. Every action lands on a SHA-256 hash chain, signed with Ed25519 — offline-verifiable by anyone in ~30 seconds, no account. Irreversible clicks stay human.

- Read tonight's receipt: [receipt/latest.json](https://sloth.utalabs.tech/receipt/latest.json)
- Verify the chain yourself: [sloth.utalabs.tech/verify](https://sloth.utalabs.tech/verify)

## BernAudio Model 80

[**bernaudio.utalabs.tech**](https://bernaudio.utalabs.tech) · [repo](https://github.com/eddyflores100-lang/bernaudio)

Real-time professional audio measurement in the browser — RTA, spectrogram, transfer function, impulse response and SPL. The free alternative to Smaart.

## Protocols & tools

- **[alethech](https://github.com/eddyflores100-lang/alethech)** — verifiable agent continuity: Ed25519-signed memory, hash-linked DAG, key rotation with reachability guarantee. Local-first, zero-LLM, zero-blockchain. Docs: [alethech.alicelabs.site](https://alethech.alicelabs.site). Listed in [Awesome-Agent-Memory](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory) after a maintainer audit of the claims against the code.
- **[universal-trust-adapter](https://github.com/alicelabs-llc/universal-trust-adapter)** — ATC/1.0 protocol spec + reference impl (Ed25519, RFC 8785 JCS, 10 verification controls). One-command conformance: `npx @marketnow/uta-conformance` (36 published vectors). Listed in [awesome-agent-native-services](https://github.com/haoruilee/awesome-agent-native-services) after review ([PR #229 merged](https://github.com/haoruilee/awesome-agent-native-services/pull/229)).
- **[marketnow-mcp](https://github.com/eddyflores100-lang/marketnow-mcp)** — free trust layer for AI agents over MCP: verify credentials (8 formats), scam-check domains, fingerprint tools. Live: [marketnow.site/api/mcp](https://www.marketnow.site/api/mcp). Listed on [mcp.so](https://mcp.so/servers/marketnow).
- **[sloptotal](https://github.com/eddyflores100-lang/sloptotal)** — open-source AI text detector: 23 engines, one calibrated score, every number measured on a public benchmark. Self-hosted, CPU-only. Live: [sloptotal.com](https://sloptotal.com).
- **[mcp-suite](https://github.com/eddyflores100-lang/mcp-suite)** — 229 MCP servers mapped to real agent pains: 1,035 tools, 349 functional tests.

## Contributions

- **[yunaremaia/mcp-guard](https://github.com/yunaremaia/mcp-guard)** — 3 merged PRs: npm attestation/provenance verification with strict policy, CLI exit-code fix on empty scans, whole-word matching for write/destructive keywords.
- **[run-llama/llama_index](https://github.com/run-llama/llama_index/pull/23352)** — open PR: simple fusion builds fresh wrappers instead of mutating retriever-owned ones.
- **[cognicore-dev/cognicore-env](https://github.com/cognicore-dev/cognicore-env)** — open PRs: lexical-search score bounds in the SQLite memory backend, verifier-defeat chain topology tests.
- **[x402-foundation/x402](https://github.com/x402-foundation/x402/issues/3803)** — spec work on the PAYMENT-REQUIRED schema: falsy-value rule re-scoped to examples with named-path failure reasons and `unavailable` as a third verdict in the redraft.
- **[taikotalent-phishing-iocs](https://github.com/eddyflores100-lang/taikotalent-phishing-iocs)** — published IoCs and attack-chain writeup for a live fake-recruiter campaign ([dev.to writeup](https://dev.to/edison_flores_6d2cd381b13/a-fake-recruiter-sent-me-a-job-offer-that-ended-in-my-terminal-the-trojan-is-still-live-2okf)).

## Writing

Long-form series on building agent trust infrastructure — what a maintainer audit actually checks, and the honest accounting of what listings pay: [dev.to/edison_flores_6d2cd381b13](https://dev.to/edison_flores_6d2cd381b13)

## Contact

[utalabs.tech](https://utalabs.tech) · [alicelabs.site](https://alicelabs.site) · AliceLabs LLC — Wyoming, USA · Quito, Ecuador
