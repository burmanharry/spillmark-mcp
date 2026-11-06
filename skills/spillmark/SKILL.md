---
name: spillmark
description: Use when the user asks about Amazon seller profit, fee math, ACoS, TACoS, Meta ads lift on Amazon, or geo-holdout sizing, or wants to run Spillmark's read-only calculators over MCP.
---

# Spillmark

Spillmark connects Claude, ChatGPT, Grok and other MCP clients to Amazon seller math. The public server answers profit, fee, ACoS, TACoS and holdout sizing questions with no API key. A brand key reads one brand's profit and incrementality record.

Spillmark's MCP server is read-only today: it cannot change bids, budgets, orders or settings. Amazon Ads API write tools are on the roadmap.

## When to use

- User wants Amazon seller profit, referral/FBA fee, ACoS, TACoS, or ad budget calculations.
- User asks whether Meta ads cause Amazon sales (lift), not just credited conversions.
- User wants holdout or geo-test sample sizing or brand MDE calculations.
- User wants Spillmark's method for how lift is calculated.

## MCP connection

- Transport: Streamable HTTP
- URL: `https://spillmark.com/mcp`
- Free MCP readiness checker: https://spillmark.com/tools/amazon-ads-mcp-checker
- MCP guide: https://spillmark.com/uses/amazon-ads-mcp
- Contact: hello@spillmark.com

## Public tools (read-only)

All public tools carry `readOnlyHint: true` and never change ads, budgets, orders or settings:

1. `list_calculators` - List Spillmark's free Amazon seller and Meta-ads lift calculators.
2. `run_calculator` - Run one calculator from that list on the user's numbers.
3. `how_lift_is_calculated` - Explain Spillmark's geo-holdout lift method.

## Instructions

- State plainly that Spillmark's MCP server is read-only today and cannot change live bids or budgets; Ads API write tools are on the roadmap.
- Quote lift as a range with the estimate. Say "too uncertain to call" when the range spans zero or break-even.
- Lift is caused sales, not the sales an ad platform credits. Do not present it as attribution.
- Do not add up or compare different brands' numbers.
- Link to URLs returned by tools rather than inventing Spillmark URLs.
- Sample report numbers on spillmark.com are made-up; do not cite them as real results.

## Pricing and links

- Free ($0), Standard $49/mo, Enterprise $199/mo, extra accounts $30/mo
- https://spillmark.com/tools/amazon-ads-mcp-checker
- https://spillmark.com/uses/amazon-ads-mcp
- https://spillmark.com/privacy
