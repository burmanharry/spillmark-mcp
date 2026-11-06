# Spillmark MCP

Remote [Model Context Protocol](https://modelcontextprotocol.io) server for [Spillmark](https://spillmark.com).

Spillmark's MCP server at `https://spillmark.com/mcp` is read-only today. Public Amazon profit, referral/FBA fee, ACoS, TACoS, and geo-holdout calculators require no key. An optional `sm_...` brand key reads a brand's own profit and incrementality record. Amazon Ads API write tools are on the roadmap.

- **Server URL:** `https://spillmark.com/mcp` (Streamable HTTP)
- **MCP guide:** https://spillmark.com/uses/amazon-ads-mcp
- **Amazon Ads MCP Checker:** https://spillmark.com/tools/amazon-ads-mcp-checker
- **Agents:** https://spillmark.com/agents
- **Privacy:** https://spillmark.com/privacy
- **Repository:** https://github.com/burmanharry/spillmark-mcp
- **Registry name:** `com.spillmark/spillmark`
- **License:** MIT (this listing repo)

This repository is the public listing package: registry and directory manifests, install snippets, and assets.

## Connect (public tools, no key)

### Cursor (`.cursor/mcp.json` or `.mcp.json`)

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

### Gemini CLI

This repo includes `gemini-extension.json` and `GEMINI.md`. The extension connects to `https://spillmark.com/mcp`.

## Brand tools (optional key)

Create a read-only key in Spillmark Settings -> Agent access, then send:

`Authorization: Bearer sm_...`

The key reads that brand's own profit and incrementality record. No tool changes ads, budgets, orders, or settings. Public calculators work without a key.

## Listing files

| File | Consumer |
| --- | --- |
| `server.json` | Official MCP Registry |
| `glama.json` | Glama |
| `smithery.yaml` | Smithery |
| `plugin.json` | Agent Plugins / Cursor Directory |
| `.cursor-plugin/plugin.json` | Cursor Directory |
| `mcp.json`, `.mcp.json` | MCP clients |
| `gemini-extension.json`, `GEMINI.md` | Gemini CLI |
| `skills/spillmark/SKILL.md` | Agent skill crawlers |

## Categories / tags

Marketing, advertising, Amazon Ads, seller profit, referral and FBA fees, ACoS, TACoS, geo-holdout, incrementality, calculators, e-commerce.

## Privacy

https://spillmark.com/privacy
