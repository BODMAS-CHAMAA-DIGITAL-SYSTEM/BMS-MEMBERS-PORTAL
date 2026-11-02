# Security Policy

## Reporting a vulnerability

Do not publish exploitable vulnerabilities, credentials, personal data, or
production system details in a public issue. Report suspected security issues
privately to the authorised BODMAS CHAMA project maintainer using a verified
contact channel supplied by the organisation. Include the affected component,
impact, reproduction steps and any relevant timestamps. Do not include real
member passwords, identity documents or payment credentials.

## Security requirements

- Keep secrets in the hosting provider's secret/environment-variable store.
- Require HTTPS for deployed applications and service endpoints.
- Enforce authentication and role permissions on the server and database.
- Apply least-privilege access and review privileged accounts regularly.
- Validate and audit sensitive financial and administrative operations.
- Never commit production data, database dumps, tokens or private documents.
- Use synthetic data in development, tests and issue reports.
