# Ready To Submit

## Already done in code/package

- unified public connector URL: `https://mcp-v1.findem.ai/mcp`
- one public app name: `Findem Studio`
- OAuth-protected MCP surface
- tool safety metadata in the backend
- submission copy in `OPENAI_SUBMISSION.md`
- private test instructions in `CONNECT_CHATGPT.md`

## Human-only items still required

1. Create a reviewer/demo account with sample data.
2. Make sure that account has no MFA or 2FA enabled.
3. Test the connector in ChatGPT web.
4. Test the connector in ChatGPT mobile.
5. Capture screenshots of:
   - connector creation
   - OAuth login
   - successful tool usage
6. Paste the fields from `OPENAI_SUBMISSION.md` into the OpenAI submission form.

## Suggested final smoke test

1. Add connector URL: `https://mcp-v1.findem.ai/mcp`
2. Authenticate with the demo account.
3. Run:
   - `Find senior product marketers in San Francisco who worked at developer-tools companies.`
   - `Find recruiting software companies between 200 and 2000 employees and summarize their hiring signals.`
   - `Who joined Stripe as a product manager in 2018?`
