# AgentaOS Documentation

Official documentation for AgentaOS — the financial OS for the agent economy.

**Live docs:** [docs.agentaos.ai](https://docs.agentaos.ai)

## Products

| Product | Description | Status |
|---------|-------------|--------|
| [Agenta Wallet](./guardian) | 2-of-3 threshold signing for AI agents — CLI, SDK, MCP | Live |
| [x402 Facilitator](./x402) | Payment verification and settlement for x402 protocol | Live |

## AI-Friendly Docs

This documentation is optimized for AI agent consumption. Mintlify auto-generates `llms.txt` and `llms-full.txt` at the site root for LLM context ingestion. You can also use the individual `.mdx` files directly.

**Key files for AI agents:**
- `guardian/integration/sdk.mdx` — SDK integration (packages, classes, methods)
- `guardian/integration/cli.mdx` — CLI commands reference
- `guardian/integration/mcp.mdx` — MCP server tools for Claude/Cursor
- `guardian/quickstart.mdx` — End-to-end setup guide

## Development

```bash
npx mintlify dev
```

Docs at `http://localhost:3000`

## Project Structure

```
├── mint.json           # Mintlify configuration
├── guardian/           # Agenta Wallet docs
│   ├── introduction.mdx
│   ├── quickstart.mdx
│   ├── integration/    # CLI, SDK, MCP, Foundry
│   ├── concepts/       # Threshold signing, guardrails, security
│   └── comparisons/    # vs Fireblocks, vs Privy, MPC vs Multisig
├── x402/               # x402 Payment Facilitator docs
│   ├── introduction.mdx
│   ├── quickstart.mdx
│   ├── api-reference/
│   └── integration/
└── images/             # Logos and assets
```

## License

[MIT](./LICENSE)
