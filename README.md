# Bms Members Portal

> Secure member portal for BODMAS CHAMA, enabling members to manage profiles, contributions, savings, loans, repayments, statements, documents, and account notifications.

## Purpose

The authenticated self-service portal for registered BODMAS CHAMA members.

## Responsibilities

- Display the authenticated member dashboard and personal account information.
- Provide access to contributions, savings, loans, repayments, statements and notifications.
- Allow members to submit permitted requests and view the status of those requests.
- Consume authorised data and actions through the central BMS API.

## Out of scope and security boundaries

- Never trust a member ID, role, balance or payment status supplied by the browser.
- Do not place service-role keys, database passwords or private credentials in frontend code.

## Architecture

This repository is one independently versioned component of the BODMAS CHAMA
hybrid digital architecture. It integrates with the central BMS API and other
services through documented, version-controlled interfaces. It is not a
standalone replacement for the complete BODMAS CHAMA system.

## Local development

1. Clone this repository.
2. Read the component-specific instructions in this README and `docs/`.
3. Copy `.env.example` to `.env` only when environment variables are required.
4. Use synthetic development data and non-production credentials.
5. Run the checks documented by this component before committing.

Do not commit `.env`, credentials, production database files or real member data.

## Deployment

This repository is intended for independent deployment. Configure the hosting provider to publish the `docs` directory. The accompanying `netlify.toml` sets this publish directory as a starting configuration. Confirm the custom domain, HTTPS, environment configuration and deploy preview settings in the hosting dashboard.

## Repository conventions

- Keep changes limited to this component's responsibility.
- Document API, data model or configuration changes.
- Coordinate breaking changes with dependent repositories.
- Use pull requests and review security-sensitive changes before release.

## Related repositories

- `BMS-PUBLIC-SITE`
- `BMS-MEMBERS-PORTAL`
- `BMS-ADMIN-PORTAL`
- `BMS-API-SERVICE`
- `BMS-HOOK-SERVICE`
- `BMS-CLIENTS-PORTAL`
- `BMS-CDN-ASSETS`
- `BMS-DATABASE`

## Ownership and licence

See [LICENSE](LICENSE) and [SECURITY.md](SECURITY.md).
