# Findem Studio OpenAI Connectors

This repository contains the OpenAI Apps / ChatGPT submission materials for Findem Studio's production MCP surfaces.

## Current production connector shape

OpenAI's ChatGPT connector flow expects a single MCP server URL per connector. Findem Studio currently exposes three production MCP endpoints, so the clean current packaging is three ChatGPT connectors:

- `findem-people` -> `https://mcp-v1.findem.ai/services/findem-people`
- `findem-companies` -> `https://mcp-v1.findem.ai/services/findem-companies`
- `findem-tempo` -> `https://mcp-v1.findem.ai/services/findem-tempo`

If you later want one single OpenAI app listing called `Findem Studio`, the backend should expose a unified top-level `/mcp` endpoint that bundles all of the public tools behind one connector URL.

## Shared production links

- Docs and examples: `https://studio.findem.ai/mcps`
- Privacy policy: `https://www.findem.ai/privacy-policy-corp`
- Support: `support@findem.ai`

## Repository layout

- `OPENAI_SUBMISSION.md`
- `CONNECT_CHATGPT.md`
- `connector-catalog.json`
- `connectors/findem-people.md`
- `connectors/findem-companies.md`
- `connectors/findem-tempo.md`
