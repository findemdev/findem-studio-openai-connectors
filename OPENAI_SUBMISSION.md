# Findem Studio OpenAI Submission Packet

This packet is for submitting Findem Studio to OpenAI using the current production MCP topology.

## Recommended submission strategy

Submit three ChatGPT connectors now:

- `Findem People`
- `Findem Companies`
- `Findem Tempo`

Reason: ChatGPT connector creation uses a single connector URL per app/connector, and Findem's current production deployment exposes three distinct MCP server URLs rather than one unified `/mcp` entry point.

## Shared listing fields

- Publisher / brand:
  - `Findem`
- Homepage:
  - `https://studio.findem.ai/mcps`
- Privacy policy:
  - `https://www.findem.ai/privacy-policy-corp`
- Support:
  - `support@findem.ai`
- Privacy contact:
  - `privacy@findem.ai`

## Shared review requirements

- All tools must have correct `readOnlyHint`, `destructiveHint`, and explicit `openWorldHint`.
- Because Findem tools operate within a closed private SaaS system, `openWorldHint` should remain explicit and `false` for the private Findem tools. Public web fetch behavior should remain explicitly marked when applicable.
- Provide a fully featured demo account with sample data and no MFA.
- Verify behavior on ChatGPT web and mobile before submission.

## Connector list

### Findem People

- Connector name:
  - `Findem People`
- Connector URL:
  - `https://mcp-v1.findem.ai/services/findem-people`
- Description:
  - `Search talent, resolve people, analyze candidate pools, create scorecards, and review candidate details using Findem's recruiting and people-search tools.`

### Findem Companies

- Connector name:
  - `Findem Companies`
- Connector URL:
  - `https://mcp-v1.findem.ai/services/findem-companies`
- Description:
  - `Research companies, resolve company identities, inspect taxonomy, and retrieve company intelligence from Findem.`

### Findem Tempo

- Connector name:
  - `Findem Tempo`
- Connector URL:
  - `https://mcp-v1.findem.ai/services/findem-tempo`
- Description:
  - `Answer historical workforce questions such as who worked at a company in a given year, who joined in a given year, or who left in a given year.`

## Reviewer account

- Demo account email:
  - `TBD`
- Demo account password:
  - `TBD`
- Notes:
  - no MFA
  - include sample data that exercises People, Companies, and Tempo

## Example prompts

- People:
  - `Find senior product marketers in San Francisco who worked at developer-tools companies.`
- Companies:
  - `Find recruiting software companies between 200 and 2000 employees.`
- Tempo:
  - `Who joined Stripe as a product manager in 2018?`

## Future simplification

If Findem later exposes one unified production `/mcp` endpoint, replace the three-connector strategy above with one `Findem Studio` app submission.
