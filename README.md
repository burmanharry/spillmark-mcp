# Spillmark MCP

Remote [Model Context Protocol](https://modelcontextprotocol.io) server for [Spillmark](https://spillmark.com): free Amazon and Meta ads calculators, and (with a read-only brand key) a brand’s own holdout-test lift, test plans, and locked predictions.

- **Server URL:** `https://spillmark.com/mcp` (Streamable HTTP)
- **Homepage / docs:** https://spillmark.com/agents
- **Registry name:** `com.spillmark/spillmark`
- **License:** MIT (this listing repo)

The product app lives elsewhere. This repository is the public listing package: `server.json`, install snippets, and assets for MCP directories.

## Connect (public tools — no key)

### Cursor (`.cursor/mcp.json`)

```json
{
  "mcpServers": {
    "spillmark": {
      "url": "https://spillmark.com/mcp"
    }
  }
}
```

### Claude Code

```bash
claude mcp add --transport http spillmark https://spillmark.com/mcp
```

### Claude / ChatGPT

Add a custom connector / MCP server with URL `https://spillmark.com/mcp`.

## Brand tools (optional key)

Create a read-only key in Spillmark **Settings → Agent access**, then send:

`Authorization: Bearer sm_…`

No tool changes ads, budgets, or settings. Public calculators work without a key.

## Categories / tags

Marketing, advertising, Amazon, Meta ads, ROAS, holdout tests, incrementality, calculators, e-commerce.

## Privacy

https://spillmark.com/privacy
