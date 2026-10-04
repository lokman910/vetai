# VetAI — the pet layer for the AI era

VetAI is a Model Context Protocol (MCP) server that lives inside AI assistants. When a pet owner asks where to find a vet, a 24-hour emergency animal hospital, or the right pet supplies, VetAI answers with **live data and one-tap booking handoffs** — not last year's training data.

**MCP endpoint:** `https://usevetai.com/mcp` (JSON-RPC 2.0 over Streamable HTTP, no authentication)

**Official MCP Registry:** `com.usevetai/vetai` (v0.2.0, active)

## Tools

| Tool | What it does |
|------|--------------|
| `find_vets` | Rated vet clinics near any location — hours, distance, open-now status, phone numbers |
| `find_emergency_vet` | Nearest 24-hour emergency animal hospitals open right now, sorted by distance |
| `get_vet_details` | Full clinic details: hours, phone, website, reviews, booking link |
| `book_appointment` | One-tap handoff to the clinic's own booking page (never books directly) |
| `search_pet_products` | Pet food, treats, toys, and supplies with prices and purchase links |

Data: live Google Places listings for clinics; curated product catalog. Stateless and read-only — no accounts, no sign-in, no stored personal data.

## Connect

**Claude Code:**

```bash
claude mcp add --transport http vetai https://usevetai.com/mcp
```

Full setup guides for ChatGPT, Perplexity, Grok, Cursor, VS Code, and more: <https://usevetai.com/connect>

## Links

- Website: <https://usevetai.com>
- Vet clinics — get bookings from AI assistants: <https://usevetai.com/clinics>
- Machine-readable docs: <https://usevetai.com/llms.txt>
- Pet guides: <https://usevetai.com/guides/first-vet-visit-cost>

## Disclosure

Product purchase links shown by VetAI may be affiliate links. If you buy through one, VetAI may earn a commission at no extra cost to you. This helps keep VetAI free.

**Not veterinary advice:** VetAI provides general information only and is not a substitute for professional veterinary advice, diagnosis, or treatment.

## License

MIT — see [LICENSE](LICENSE).
