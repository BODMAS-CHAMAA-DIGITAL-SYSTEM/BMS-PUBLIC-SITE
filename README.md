# Bms Public Site

> Official public website for BODMAS CHAMA, providing organisational information, membership details, savings, loans, investments, projects, announcements, and contact resources.

## Purpose

The public-facing website for BODMAS CHAMA.

## Responsibilities

- Present verified organisational information and public announcements.
- Explain membership, savings, loan, investment and project information.
- Provide contact details, public resources and application entry points.
- Link users to the member, administration and partner portals where appropriate.

## Out of scope and security boundaries

- Do not store member account data or private documents in this repository.
- Do not implement financial posting or payment verification in browser JavaScript.

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
