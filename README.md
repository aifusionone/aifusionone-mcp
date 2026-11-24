# AI Fusion One — pay-per-call data & verification API for AI agents

Remote MCP server + HTTP API. 23 tools (weather alerts, hazards, wildfires, product & vehicle recalls, SEC company filings, treasury rates, economic indicators, energy prices, ag stats, space weather, port conditions, cyber threats, web checks, trade rules, supplier matching and more).

- **Pricing:** from $0.05 per call, paid per request with [x402](https://x402.org) (USDC on Base). No account needed.
- **Free test keys:** https://theaiworldnetwork.com/docs#signup
- **API base:** https://aifusionone.allaihq.workers.dev
- **MCP endpoint (streamable HTTP):** https://aifusionone.allaihq.workers.dev/mcp
- **OpenAPI:** https://aifusionone.allaihq.workers.dev/openapi.json
- **LLM guide:** https://aifusionone.allaihq.workers.dev/llms.txt
- **Pricing list:** https://aifusionone.allaihq.workers.dev/v1/pricing

## MCP client config

```json
{
  "mcpServers": {
    "aifusionone": { "url": "https://aifusionone.allaihq.workers.dev/mcp" }
  }
}
```

## Quick test

```bash
curl -i https://aifusionone.allaihq.workers.dev/v1/services
```

Paid routes answer `402 Payment Required` with x402 v1 and v2 payment details; any x402 client can pay and retry.

Operated by All AI LLC. Contact: open an issue at https://github.com/aifusionone/aifusionone-mcp/issues
