# Eddy Flores — AliceLabs LLC

**Trust infrastructure for AI agents.** Receipts, not vibes.

I build the full stack that answers one question: *should this agent be allowed to do that?* Identity, translation, audit, enforcement — every claim on this page links to a repo, a live receipt or a spec. Nothing here is a vibe.

**Live:** [marketnow.site](https://marketnow.site) — the registry · [utalabs.tech](https://utalabs.tech) — the stack · [alicelabs.site](https://alicelabs.site) — the company

[![XERJ Corpus Hub contributor](https://hub.xerj.org/contributors/eddyflores100-lang/badge.svg)](https://hub.xerj.org/contributors/eddyflores100-lang) [![Hacktoberfest 2026 Completionist](https://img.shields.io/badge/Hacktoberfest_2026-Completionist-181717?logo=hacktoberfest&logoColor=white)](https://dev.to/edison_flores_6d2cd381b13) [![FLISK HALL OF FAME @eddyflores100-lang • 1 merged PR](https://img.shields.io/badge/FLISK%20HALL%20OF%20FAME-%40eddyflores100_lang%20%E2%80%A2%201%20merged%20PR-00D1FF?labelColor=07080f)](https://github.com/flisk-sh/flisk/issues?q=is%3Aissue+is%3Aopen+label%3Acommunity) [![Founding Contributor #8 @arxh80](https://img.shields.io/static/v1?label=%E2%9A%A1%20FOUNDING%20CONTRIBUTOR&message=%238%20of%20100%20%E2%80%A2%20%40arxh80&color=00D1FF&labelColor=07080f)](https://discord.gg/qMu5Xn8Kaq) [![PRs merged](https://img.shields.io/badge/PRs_merged-74_%C2%B7_Nov_2026-00D1FF?labelColor=07080f)](https://github.com/search?q=type%3Apr+author%3Aeddyflores100-lang+is%3Amerged)

[![MarketNow on mcptry](https://mcptry.com/badge/io.github.alicelabs-llc/marketnow.svg)](https://mcptry.com/servers/io.github.alicelabs-llc/marketnow) [![marketnow-mcp downloads](https://img.shields.io/npm/dm/marketnow-mcp?label=marketnow-mcp&color=00D1FF)](https://www.npmjs.com/package/marketnow-mcp) [![uta-conformance downloads](https://img.shields.io/npm/dm/@marketnow/uta-conformance?label=%40marketnow%2Futa-conformance&color=00D1FF)](https://www.npmjs.com/package/@marketnow/uta-conformance) [![status](https://img.shields.io/website?url=https%3A%2F%2Fstatus.marketnow.site&label=status)](https://status.marketnow.site)

---

## Track record — Nov 2026

- **74 PRs merged** — 30 into 20 external repositories, 44 into AliceLabs repos. Selected: [punkpeye/awesome-mcp-servers #16284](https://github.com/punkpeye/awesome-mcp-servers/pull/16284) (97k+ star repo), [useagenthq/useagent](https://github.com/useagenthq/useagent) ×5, [cognicore-dev/cognicore-env](https://github.com/cognicore-dev/cognicore-env) ×7, [flisk-sh/flisk #951](https://github.com/flisk-sh/flisk/pull/951) (Hall of Fame), [floatpane/matcha #1733](https://github.com/floatpane/matcha/pull/1733) (completed the Spanish translation), [meetdino/dino #124](https://github.com/meetdino/dino/pull/124).
- **57 issues filed** — headlined by a fail-closed spend-authority proposal series to agent-wallet teams: [microsoft/autogen #8377](https://github.com/microsoft/autogen/issues/8377), [crewAIInc/crewAI #8381](https://github.com/crewAIInc/crewAI/issues/8381), [safe-global/safe-core-sdk #1453](https://github.com/safe-global/safe-core-sdk/issues/1453), [tkhq/sdk (Turnkey) #1622](https://github.com/tkhq/sdk/issues/1622), [privy-io/aws-agentcore-sdk #10](https://github.com/privy-io/aws-agentcore-sdk/issues/10), [akash-network/console #4549](https://github.com/akash-network/console/issues/4549), [glama-ai/lightport #15](https://github.com/glama-ai/lightport/issues/15) — plus [x402-foundation/x402 #3803](https://github.com/x402-foundation/x402/issues/3803) on the PAYMENT-REQUIRED schema.
- **47 PRs open** — distribution in flight: MarketNow into [docker/mcp-registry #5263](https://github.com/docker/mcp-registry/pull/5263) (local + remote), [xai-org/plugin-marketplace #1012](https://github.com/xai-org/plugin-marketplace/pull/1012), [solana-foundation/pay #525](https://github.com/solana-foundation/pay/pull/525), [browser-use #6226](https://github.com/browser-use/browser-use/pull/6226), [run-llama/llama_index #23758](https://github.com/run-llama/llama_index/pull/23758), plus 15+ curated lists.
- **2 packages on npm**: [marketnow-mcp](https://www.npmjs.com/package/marketnow-mcp) — free trust layer for MCP agents (1.1k downloads last month) · [@marketnow/uta-conformance](https://www.npmjs.com/package/@marketnow/uta-conformance) — signed ATC/1.0 conformance vectors.
- **Registry & audit numbers**: 71,198+ MCP servers indexed on [marketnow.site](https://marketnow.site) · Sentinel: 1,211,488 checks, 1,030 threats caught · [mcptry 96/100, #454 of 4,704](https://mcptry.com/servers/io.github.alicelabs-llc/marketnow) in AI & Agents.

## The utalabs.tech stack

Four files, one question. Each product answers it at a different layer.

| Layer | Product | What it is | Proof |
|---|---|---|---|
| 01 · translation | [**UTA**](https://utalabs.tech/uta/) — universal trust adapter | 8 credential formats in (JWT, W3C VC, A2A, X.509, ATC…), one canonical schema out. 12-stage verification pipeline. | [x402 API](https://uta-trust-api.eddyflores100.workers.dev) — $0.01/verify, fail-closed · [spec + repo](https://github.com/alicelabs-llc/universal-trust-adapter) |
| 02 · identity | [**ATC**](https://utalabs.tech/atc/) — agent trust card | Ed25519-signed capability card (ATC/1.0, RFC v3.0): who the agent is, what it may touch, who answers for it. | 57 cards live · MNR-CRL-1.0 revocation · [spec + repo](https://github.com/alicelabs-llc/universal-trust-adapter) |
| 03 · audit | [**Sentinel**](https://utalabs.tech/sentinel/) | 10 static layers + a real L2 sandbox: every MCP server executed under gVisor, syscalls watched for 30 s. | 1,211,488 checks · 1,030 threats caught |
| 04 · enforcement | [**Interceptor**](https://utalabs.tech/interceptor/) | MCP runtime policy engine. Blocks `.env` reads and `rm -rf` even when the caller's card is valid. | 5 live rules · signed JSONL audit trail |
| annex A · provider side | [**UTA-Shield**](https://wall.utalabs.tech) — firewall for MCP operators | Wraps your MCP server once: identity gates, threat-intel blocking (23 live IOCs from a real takedown), rate limits, DLP, x402 metering. 19.8 kB, zero dependencies. | [repo](https://github.com/eddyflores100-lang/uta-shield) |
| annex B · registry | [**MarketNow**](https://marketnow.site) | Security infrastructure for AI agents: skills, credentials and domains verified across 71,198 MCP servers indexed. | free MCP API, 10 tools, no signup · [repo](https://github.com/eddyflores100-lang/marketnow) · [status](https://status.marketnow.site) |

Fail-closed is the house rule: unreachable revocation check → DENY. Downtime degrades to "no", never to "probably fine".

## SLOTH — the overnight agent that hands you a receipt

[**sloth.utalabs.tech**](https://sloth.utalabs.tech) · [repo](https://github.com/eddyflores100-lang/sloth)

**S**leepy **L**azy **O**vernight **T**ask **H**andler. A 1B open-weight brain (Gemma 3 + llama.cpp) that runs on your CPU and does the boring stuff while you sleep. Every action lands on a SHA-256 hash chain, signed with Ed25519 — offline-verifiable by anyone in ~30 seconds, no account. Irreversible clicks stay human.

- Read tonight's receipt: [receipt/latest.json](https://sloth.utalabs.tech/receipt/latest.json)
- Verify the chain yourself: [sloth.utalabs.tech/verify](https://sloth.utalabs.tech/verify)

## MarketNow — the trust registry

[**marketnow.site**](https://marketnow.site) · [status](https://status.marketnow.site) · [repo](https://github.com/eddyflores100-lang/marketnow)

Where the stack meets the world: security infrastructure for AI agents — skills, credentials and domains verified across **71,198 MCP servers indexed** (135,547 tracked), with a **free MCP API** — 10 tools, no keys, no signup — plus signed submissions, revocation checks and a Sentinel score on every entry.

- Free API: [marketnow.site/api/mcp](https://marketnow.site/api/mcp)
- Live status: [status.marketnow.site](https://status.marketnow.site)
- Agent surface: [uta-ai](https://github.com/alicelabs-llc/uta-ai) — installable skills, subagents, MCP servers, Claude Code plugin

## Protocols, tools & side builds

- **[alethech](https://github.com/eddyflores100-lang/alethech)** — verifiable agent continuity: Ed25519-signed memory, hash-linked DAG, key rotation with reachability guarantee. Local-first, zero-LLM, zero-blockchain. Docs: [alethech.alicelabs.site](https://alethech.alicelabs.site). Listed in [Awesome-Agent-Memory](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory) after a maintainer audit of the claims against the code.
- **[universal-trust-adapter](https://github.com/alicelabs-llc/universal-trust-adapter)** — ATC/1.0 protocol spec + reference impl (Ed25519, RFC 8785 JCS, 10 verification controls). One-command conformance: `npx @marketnow/uta-conformance` (36 published vectors). Listed in [awesome-agent-native-services](https://github.com/haoruilee/awesome-agent-native-services) after review ([PR #229 merged](https://github.com/haoruilee/awesome-agent-native-services/pull/229)).
- **[marketnow-mcp](https://github.com/eddyflores100-lang/marketnow-mcp)** — free trust layer for AI agents over MCP: verify credentials (8 formats), scam-check domains, fingerprint tools. Live: [marketnow.site/api/mcp](https://marketnow.site/api/mcp). Listed on [mcp.so](https://mcp.so/servers/marketnow).
- **[sloptotal](https://github.com/eddyflores100-lang/sloptotal)** — open-source AI text detector: 23 engines, one calibrated score, every number measured on a public benchmark. Self-hosted, CPU-only. Live: [sloptotal.com](https://sloptotal.com).
- **[mcp-suite](https://github.com/eddyflores100-lang/mcp-suite)** — 229 MCP servers mapped to real agent pains: 1,035 tools, 349 functional tests.
- **[BernAudio Model 80](https://bernaudio.utalabs.tech)** — real-time professional audio measurement in the browser: RTA, spectrogram, transfer function, impulse response, SPL. Free alternative to Smaart. [repo](https://github.com/eddyflores100-lang/bernaudio)

## Hackathons

- **[alethech-agent-vault](https://github.com/eddyflores100-lang/alethech-agent-vault)** — Vultr Agent Rush (Nov 3–8, 2026): verifiable agent execution on Vultr; every agent action signed via alethech.
- **[mailhand-aws-cds](https://github.com/eddyflores100-lang/mailhand-aws-cds)** — AWS CDS Agentic AI Partner Hackathon (Oct 28, 2026): agentic email code review via AWS SES + Bedrock AgentCore.
- **[mermail-escrow-agent](https://github.com/eddyflores100-lang/mermail-escrow-agent)** — Mermail Build & Demo bounty: peer-to-peer escrow over a Mermail email thread — buyer funds held in Agent Wallet, released to the seller only after buyer email confirmation (USDC).
- **[zolo-qloo-agent](https://github.com/alicelabs-llc/zolo-qloo-agent)** — Qloo hackathon submission: conversational cultural-discovery agent on Cloudflare Workers AI.

## Open source — merged (selected)

- **[useagenthq/useagent](https://github.com/useagenthq/useagent)** — 5 merged PRs: axe accessibility sweep across the five main pages with fixes, desktop smoke test on the packaged app, collapse-all and jump-to-error controls in the trace view, content-aware waits, package README.
- **[cognicore-dev/cognicore-env](https://github.com/cognicore-dev/cognicore-env)** — 7 merged PRs: quarantine-backend flush at end of import_bundle, lexical-search score bounds in the SQLite backend, verifier-defeat chain topology tests, CI dependency and mock fixes.
- **[punkpeye/awesome-mcp-servers #16284](https://github.com/punkpeye/awesome-mcp-servers/pull/16284)** — alethech listed under Knowledge & Memory after maintainer review.
- **[profullstack/x402-gateway #23](https://github.com/profullstack/x402-gateway/pull/23)** — x402 verification badge endpoint for external indexers.
- **[Podiom/Podiom #380](https://github.com/Podiom/Podiom/pull/380)** — MCP pin dedupe merge semantics with focused tests.
- **[aniruddhaadak80/skills #471](https://github.com/aniruddhaadak80/skills/pull/471)** — Ed25519 skill verification badges (sign + verify).
- **[taikotalent-phishing-iocs](https://github.com/eddyflores100-lang/taikotalent-phishing-iocs)** — published IoCs and attack-chain writeup for a live fake-recruiter campaign ([dev.to writeup](https://dev.to/edison_flores_6d2cd381b13/a-fake-recruiter-sent-me-a-job-offer-that-ended-in-my-terminal-the-trojan-is-still-live-2okf)).

## In review — open PRs (selected)

- **[run-llama/llama_index #23758](https://github.com/run-llama/llama_index/pull/23758)** — optional trust-verification middleware for MCP servers; companion fix [#23352](https://github.com/run-llama/llama_index/pull/23352) (simple fusion builds fresh wrappers instead of mutating retriever-owned ones).
- **[browser-use/browser-use #6226](https://github.com/browser-use/browser-use/pull/6226)** — trust verification before browser tool execution.
- **[docker/mcp-registry #5263](https://github.com/docker/mcp-registry/pull/5263) · [#5175](https://github.com/docker/mcp-registry/pull/5175)** — MarketNow local and remote MCP servers.
- **[xai-org/plugin-marketplace #1012](https://github.com/xai-org/plugin-marketplace/pull/1012)** — marketnow as a remote source with pinned sha.
- **[solana-foundation/pay #525](https://github.com/solana-foundation/pay/pull/525)** — reference remote spending authority over HTTP.
- Curated lists with open submissions: [punkpeye/awesome-mcp-servers #13933](https://github.com/punkpeye/awesome-mcp-servers/pull/13933) (MarketNow) and [#17326](https://github.com/punkpeye/awesome-mcp-servers/pull/17326) (uta-shield), [punkpeye/awesome-remote-mcp-servers #1928](https://github.com/punkpeye/awesome-remote-mcp-servers/pull/1928), [x402-foundation/x402 #3815](https://github.com/x402-foundation/x402/pull/3815), and 10+ more.

## Recognition

- **Hacktoberfest 2026 Completionist badge** — awarded by DEV Community (Nov 2026), "one of Hacktoberfest 2026's top participants". Profile: [dev.to/edison_flores_6d2cd381b13](https://dev.to/edison_flores_6d2cd381b13).
- **[XERJ Corpus Hub contributor](https://hub.xerj.org/contributors/eddyflores100-lang)** — [universal-trust-adapter](https://github.com/alicelabs-llc/universal-trust-adapter) selected and indexed by the XERJ Corpus Hub (Oct 2026).
- **MarketNow on [mcptry](https://mcptry.com/servers/io.github.alicelabs-llc/marketnow)** — #454 of 4,704 in AI & Agents, score 96/100 (Nov 2026). Also listed on [mcp.so](https://mcp.so/servers/marketnow) and [mcpservers.org](https://mcpservers.org/servers/alicelabs-llc/marketnow).
- **[Flisk Hall of Fame](https://github.com/flisk-sh/flisk/pull/951)** — first merged contribution ([PR #951](https://github.com/flisk-sh/flisk/pull/951), closes #905): refactored the `project.json` file name into a `PROJECT_JSON` constant; 7 kyu rank in Flisk CLI Cove (Oct 2026).
- **Flisk Founding Contributor #8 of 100** — numbered badge reserved for the first 100 code contributors to [flisk-sh/flisk](https://github.com/flisk-sh/flisk); unlocked via the Flisk Discord (@arxh80), Nov 2026.

## Writing

Long-form series on building agent trust infrastructure — what a maintainer audit actually checks, and the honest accounting of what listings pay: [dev.to/edison_flores_6d2cd381b13](https://dev.to/edison_flores_6d2cd381b13)

## Contact

[utalabs.tech](https://utalabs.tech) · [alicelabs.site](https://alicelabs.site) · AliceLabs LLC — Wyoming, USA · Quito, Ecuador
