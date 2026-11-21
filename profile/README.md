<div align="center">

# Phideround

### The team behind RealMarketAPI: real-time market data for developers and AI agents

[Website](https://realmarketapi.com) · [Documentation](https://realmarketapi.com/en-US/docs) · [Pricing](https://realmarketapi.com/en-US/pricing) · [Playground](https://realmarketapi.com/en-US/playground) · [FAQ](https://realmarketapi.com/en-US/faq)

[![NuGet](https://img.shields.io/nuget/v/RealMarketAPI.Sdk?style=flat-square&label=NuGet&color=512BD4)](https://www.nuget.org/packages/RealMarketAPI.Sdk)
[![npm](https://img.shields.io/npm/v/realmarketapi-js-sdk-beta/beta?style=flat-square&label=npm&color=CB3837)](https://www.npmjs.com/package/realmarketapi-js-sdk-beta)
[![PyPI](https://img.shields.io/pypi/v/realmarketapi-python-sdk-beta?style=flat-square&label=PyPI&color=3775A9)](https://pypi.org/project/realmarketapi-python-sdk-beta/)
[![Agent Skills](https://img.shields.io/badge/agent%20skills-161-6366F1?style=flat-square)](https://github.com/Phideround/realmarketapi-agent-skills)

</div>

---

## RealMarketAPI

[RealMarketAPI](https://realmarketapi.com) is a hosted API for live and historical market data across forex, metals, crypto, commodities, indices and stocks. Indicators, volatility analytics and market-structure signals are computed server-side, so clients receive answers instead of raw candles to process.

| | |
|---|---|
| **Coverage** | 61 symbols: forex, metals, crypto, commodities, indices, US stocks |
| **Data** | Live prices with bid and ask, OHLCV candles on `M1` to `D1`, paged history |
| **Analytics** | 14 technical indicators, volatility regimes and heatmaps, insight scores, liquidity and stop-hunt zones |
| **Delivery** | REST, WebSocket streams, MCP server with 33 tools, Telegram bot, embeddable widgets |
| **For AI agents** | Native MCP server, 161 open-source Agent Skills, `llms.txt` and an OpenAPI spec |
| **Getting started** | Free plan with live data, not delayed data |

```bash
curl "https://api.realmarketapi.com/api/v1/price?apiKey=YOUR_API_KEY&symbolCode=XAUUSD&timeFrame=M1"
```

The API itself is a hosted service. Everything around it, listed below, is open source.

---

## Open-source ecosystem

```
                         RealMarketAPI (hosted)
              REST  ·  WebSocket  ·  MCP server  ·  OpenAPI
                                 │
     ┌──────────────┬────────────┼────────────┬──────────────┐
     SDKs       Agent Skills   Examples      Apps          Community
  .NET · JS · Py   161 skills   video series  extension,     RSS feed
                                             dashboard,     directory
                                             calculators
```

### SDKs

| Repository | Package | Description |
|---|---|---|
| [RealMarketAPI.Sdk](https://github.com/Phideround/RealMarketAPI.Sdk) | [`RealMarketAPI.Sdk`](https://www.nuget.org/packages/RealMarketAPI.Sdk) on NuGet | Official .NET SDK. Strongly typed, async, dependency injection, REST and WebSocket streams, full API coverage. |
| [RealMarketAPI.JavaScript.Sdk](https://github.com/Phideround/RealMarketAPI.JavaScript.Sdk) | [`realmarketapi-js-sdk-beta`](https://www.npmjs.com/package/realmarketapi-js-sdk-beta) on npm | JavaScript and TypeScript SDK for Node.js 20+. REST client and WebSocket client. Beta. |
| [RealMarketAPI.Python.Sdk](https://github.com/Phideround/RealMarketAPI.Python.Sdk) | [`realmarketapi-python-sdk-beta`](https://pypi.org/project/realmarketapi-python-sdk-beta/) on PyPI | Python 3.9+ SDK built on `httpx` and `websockets`. Beta. |

### AI agents

| Repository | Description |
|---|---|
| [realmarketapi-agent-skills](https://github.com/Phideround/realmarketapi-agent-skills) | 161 Agent Skills (`SKILL.md`) in 15 agent roles, from market analyst and risk manager to quant researcher and a multi-agent trading desk. Works with Claude Code, Cursor, Codex and any agent that reads the format. |

Connect any MCP client to `https://ai.realmarketapi.com/mcp` to give an assistant direct access to 33 market tools. See the [MCP docs](https://realmarketapi.com/en-US/docs/mcp).

### Examples and learning

| Repository | Description |
|---|---|
| [code-with-realmarketapi](https://github.com/Phideround/code-with-realmarketapi) | Source code for the Code with RealMarketAPI video series: a gold price widget, a React trading dashboard, a Python alert bot and a .NET backend proxy. |
| [learn-realmarketapi](https://github.com/Phideround/learn-realmarketapi) | Learning hub with trading and market-data guides. Live at [learn.realmarketapi.com](https://learn.realmarketapi.com). |

### Apps and tools

| Repository | Description |
|---|---|
| [RealMarketAPI-ChromeExtension](https://github.com/Phideround/RealMarketAPI-ChromeExtension) | Chrome extension showing live prices for crypto, forex and commodities over WebSocket. |
| [RealMarketLive](https://github.com/Phideround/RealMarketLive) | Real-time market dashboard built on the streaming API. |
| [calculator-realmarketapi](https://github.com/Phideround/calculator-realmarketapi) | Trading calculators for position size, margin, profit, risk and drawdown. Live at [calculator.realmarketapi.com](https://calculator.realmarketapi.com). |
| [realmarketapi-game](https://github.com/Phideround/realmarketapi-game) | A market mini game. Live at [game.realmarketapi.com](https://game.realmarketapi.com). |

### Community

| Repository | Description |
|---|---|
| [RealMarketFeed](https://github.com/Phideround/RealMarketFeed) | Open, community-driven directory of trading RSS feeds across crypto, forex, stocks and macro. Live at [rss.realmarketapi.com](https://rss.realmarketapi.com). |

---

## Start here

| If you want to | Go to |
|---|---|
| Make a first API call | [Getting started](https://realmarketapi.com/en-US/docs/getting-started) |
| Try requests in the browser | [Playground](https://realmarketapi.com/en-US/playground) |
| Use the API from .NET, JavaScript or Python | [SDKs](#sdks) |
| Give an AI assistant market data | [MCP server](https://realmarketapi.com/en-US/docs/mcp) and [Agent Skills](https://github.com/Phideround/realmarketapi-agent-skills) |
| Let a coding agent do the integration | [AI integration guide](https://realmarketapi.com/en-US/docs/ai-integration) |
| See working projects | [code-with-realmarketapi](https://github.com/Phideround/code-with-realmarketapi) |

---

## Contributing

Issues and pull requests are welcome on every repository listed here. Report a bug or request a feature in the repository it concerns. Each one has its own setup instructions.

For questions about the API, your account or a plan, use the [contact page](https://realmarketapi.com/en-US/contact). To report a security issue, see the [security page](https://realmarketapi.com/en-US/security) and do not open a public issue.

Never include an API key in an issue, a pull request or a commit.

---

<div align="center">

Market data is informational and is not investment advice. See the [risk warning](https://realmarketapi.com/en-US/risk-warning).

**[realmarketapi.com](https://realmarketapi.com)**

</div>
