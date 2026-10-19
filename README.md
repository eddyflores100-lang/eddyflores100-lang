# Eddy-AliceLabs

**Edison Flores — AliceLabs LLC** · Trust infrastructure for AI agents.

I build protocols and tooling that let AI agents *prove* things: who signed their memory, which credentials are real, and what changed between runs.

## Flagship

- **[alethech](https://github.com/eddyflores100-lang/alethech)** — verifiable agent continuity: Ed25519-signed memory, hash-linked DAG, key rotation with reachability guarantee. Local-first, MIT. Listed in [Awesome-Agent-Memory](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory) after a maintainer audit of the claims against the code. Docs: [alethech.alicelabs.site](https://alethech.alicelabs.site)
- **[x402-foundation/x402](https://github.com/x402-foundation/x402/issues/3803)** — spec work on the PAYMENT-REQUIRED schema (#3803): falsy-value rule re-scoped to examples with named-path failure reasons and `unavailable` as a third verdict in the redraft — edits independently re-verified by thread participants.
- **[arketnow-mcp](https://github.com/eddyflores100-lang/marketnow-mcp)** — free trust layer for AI agents using MCP: verify credentials (8 formats), scam-check domains, fingerprint tools. Live: [arketnow.site](https://marketnow.site). Listed on [mcp.so](https://mcp.so/servers/marketnow).
- **[universal-trust-adapter](https://github.com/alicelabs-llc/universal-trust-adapter)** — ATC/1.0 Agent Trust Card protocol spec + reference impl (Ed25519, RFC 8785 JCS, 10 verification controls). Live paid verifier: [UTA Trust API](https://uta-trust-api.eddyflores100.workers.dev/) — $0.01/verify via x402 on Base; one-command conformance: `npx @marketnow/uta-conformance` (36 published vectors). Listed in [awesome-agent-native-services](https://github.com/haoruilee/awesome-agent-native-services) after review ([PR #229 merged](https://github.com/haoruilee/awesome-agent-native-services/pull/229)). Write-up: [Telegraph](https://telegra.ph/UTA-Trust-API-paid-verifiable-trust-for-AI-agents-is-live-10-19)
- **[mcp-suite](https://github.com/eddyflores100-lang/mcp-suite)** — 229 MCP servers mapped to real agent pains: 1,035 tools, 349 functional tests.
- **[dropes-v2](https://github.com/eddyflores100-lang/dropes-v2)** — dropshipping ecommerce (ES/PT), React 19 + Vite 6 + Tailwind 4, checkout with verified-delivery commissions.

## Contributions

- **[yunaremaia/mcp-guard](https://github.com/yunaremaia/mcp-guard)** — 3 merged PRs: npm attestation/provenance verification with strict policy, CLI exit-code fix on empty scans, whole-word matching for write/destructive keywords.
- **[run-llama/llama_index](https://github.com/run-llama/llama_index/pull/23352)** — open PR: simple fusion builds fresh wrappers instead of mutating retriever-owned ones.
- **[cognicore-dev/cognicore-env](https://github.com/cognicore-dev/cognicore-env)** — open PRs: lexical-search score bounds in the SQLite memory backend, verifier-defeat chain topology tests.
- **[TeleAI-UAGI/Awesome-Agent-Memory](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory)** — co-authored commit landing the alethech listing (Emerging projects).

## Writing

Long-form series on building agent trust infrastructure — including what a maintainer audit actually checks, and the honest accounting of what listings pay: [dev.to/edison_flores_6d2cd381b13](https://dev.to/edison_flores_6d2cd381b13)

## Contact

[alicelabs.energy](https://alicelabs.energy) · AliceLabs LLC
