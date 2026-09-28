# AgentaOS docs (Mintlify)

Audience: founders first, many of them non-technical or working through an AI agent; developers second.

## Rules for every page

- A guide opens from the founder's side: the product's screens, in the screen's own words, with screenshots. Code (SDK, CLI, API) comes after, under its own heading.
- Before writing or reviewing a page, load these skills: `technical-writing` (with its `references/style.md`), `mintlify`, `posthog:writing-simplified-technical-english`. Finish with `reviewing-technical-prose`. For a site-wide review use `developer-docs-structure-audit`.
- No em dashes or en dashes in prose. Headings in sentence case. No "What X…" or question headings outside a FAQ. No marketing words.
- Screenshots: real product, neutral data only (no personal emails, no localhost links), 1440px wide, under `images/<area>/` with plain names, always with alt text, inside `<Frame>`.
- Quote screen text exactly as the product shows it.
- Never name another payments company or a vendor we use (Stripe, Paddle, Wise, Bridge, Didit, Radar, Link, Creem, and so on), and never compare AgentaOS to one. Write "the card processor", "our banking partner", "the identity check". API field names and values the product returns (`stripeCustomerId`, `"network": "stripe"`) stay as they are; no prose sentence names the vendor. Check before a commit: `grep -rniE "stripe|paddle|creem|\bwise\b|\bbridge\b|didit" --include='*.mdx' .`

## Checks before a commit

- `npx mint broken-links` (the two `llms*.txt` entries on agents/overview are known).
- Open the page in the local preview (`npx mintlify dev --port 3333`) and confirm every image loads.
