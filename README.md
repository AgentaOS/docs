# AgentaOS Documentation

Official documentation for AgentaOS, the Merchant of Record for AI native founders. Payments, subscriptions, invoices, tax, and payouts, all handled.

**Live docs:** [docs.agentaos.ai](https://docs.agentaos.ai)

## AI-friendly docs

Mintlify auto-generates `llms.txt` and `llms-full.txt` at the site root for LLM context ingestion. You can also read any page as raw markdown by appending `.md` to its URL, or use the `.mdx` files directly.

## Development

```bash
npx mintlify dev
```

Open the local URL Mintlify prints. To check links:

```bash
npx mintlify broken-links
```

## Structure

- `introduction.mdx` — overview
- `getting-started/` — quickstart, test mode, dashboard
- `payments/` — payment links, checkouts, subscriptions, invoices, receipts, customers, webhooks
- `sdk/` — the `@agentaos/pay` TypeScript SDK
- `cli/` — the `agenta` CLI
- `mor/` — Merchant of Record: how it works, supported countries, tax, pricing, account review
- `payouts/` — how your balance clears and pays out
- `api-reference/` — REST API (OpenAPI-driven) and error codes
- `guides/` — end-to-end walkthroughs
- `mint.json` — Mintlify configuration
- `openapi.json` — the API spec the reference renders from

## License

[MIT](./LICENSE)
