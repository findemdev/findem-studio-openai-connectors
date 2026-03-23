# Connect From ChatGPT

Use these steps for private testing in ChatGPT developer mode.

## Before you begin

- Enable developer mode in ChatGPT.
- Ensure the production connector URL is reachable over HTTPS.
- Use a Findem test account that already has sample data and does not require MFA or 2FA.

## Create the connector

1. Go to `Settings -> Connectors -> Create`.
2. Enter the connector name: `Findem Studio`.
3. Enter the connector description from `OPENAI_SUBMISSION.md`.
4. Enter the production connector URL: `https://mcp-v1.findem.ai/mcp`.
5. Save and inspect the advertised tool list.
6. Authenticate with the Findem demo or reviewer account.
7. Run at least one recruiting prompt, one company-intelligence prompt, and one workforce-history prompt.
