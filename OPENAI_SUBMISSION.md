# Findem Studio OpenAI Submission Packet

This packet is for submitting Findem Studio to OpenAI as one ChatGPT app backed by one production MCP endpoint.

## App summary

- App name:
  - `Findem Studio`
- Publisher / brand:
  - `Findem`
- Connector URL:
  - `https://mcp-v1.findem.ai/mcp`
- Homepage:
  - `https://studio.findem.ai/mcps`
- Privacy policy:
  - `https://www.findem.ai/privacy-policy-corp`
- Support:
  - `support@findem.ai`
- Privacy contact:
  - `privacy@findem.ai`
- Authentication:
  - `OAuth 2.0`

## Short description

- `Findem Studio connects ChatGPT to Findem's recruiting, company-intelligence, and workforce-history tools through one OAuth-protected MCP server.`

## Longer description

- `Findem Studio lets ChatGPT search talent, refine recruiting pools, create scorecards, inspect candidate details, research companies, analyze company metrics, and answer historical workforce questions. Users authenticate with Findem OAuth, then ChatGPT can use the enabled Findem tools from the customer's Findem account through one managed MCP connection.`

## Review requirements

- All tools must have correct `readOnlyHint`, `destructiveHint`, and explicit `openWorldHint`.
- Because Findem tools operate within a closed private SaaS system, `openWorldHint` should remain explicit and `false` for the private Findem tools. Public web fetch behavior such as job-posting fetch should remain explicitly marked when applicable.
- Provide a fully featured demo account with sample data and no MFA or 2FA.
- Verify behavior on ChatGPT web and mobile before submission.
- Capture screenshots for install, auth, and working tool usage.

## Reviewer account

- Demo account email:
  - `TBD`
- Demo account password:
  - `TBD`
- Notes:
  - no MFA or 2FA
  - include sample data that exercises recruiting, companies, and tempo workflows
  - make sure email verification is already completed before handing the account to reviewers

## Example prompts

- `Find senior product marketers in San Francisco who worked at developer-tools companies.`
- `Find recruiting software companies between 200 and 2000 employees and summarize their hiring signals.`
- `Who joined Stripe as a product manager in 2018?`

## Suggested expected outcomes

- The first prompt returns a people search plus relevant candidate results from Findem.
- The second prompt returns matching companies, company detail, and workforce or hiring metrics.
- The third prompt returns historical workforce matches from Findem Tempo.
