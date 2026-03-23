# Connect From ChatGPT

Use these steps for private testing in ChatGPT developer mode.

## Before you begin

- Enable developer mode in ChatGPT.
- Ensure the production connector URL is reachable over HTTPS.

## Create a connector

For each production surface:

1. Go to `Settings -> Connectors -> Create`.
2. Enter the connector name.
3. Enter the connector description.
4. Enter the production connector URL.
5. Save and inspect the advertised tool list.
6. Authenticate with the Findem demo or user account.
7. Run at least one prompt against the connector.

## Recommended initial connectors

- `Findem People` -> `https://mcp-v1.findem.ai/services/findem-people`
- `Findem Companies` -> `https://mcp-v1.findem.ai/services/findem-companies`
- `Findem Tempo` -> `https://mcp-v1.findem.ai/services/findem-tempo`
