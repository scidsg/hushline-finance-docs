# Hush Line Treasurer Agent

Public documentation for the Hush Line Treasurer Agent, located in a private repo here: https://github.com/scidsg/hushline-finance

The Treasurer Agent is a locally operated bookkeeping and financial workflow automation tool for Hush Line. It is designed to assist with recurring treasurer/CFO tasks such as transaction review, reconciliation support, accounting exports, report preparation, and accountant-facing summaries.

The agent code is maintained in a private repository. This public repository exists for user-facing documentation, legal terms, privacy disclosures, security notes, and project transparency.

---

## What This Repository Contains

This repository may include:

- End User License Agreement
- Privacy Policy
- user documentation
- security model notes
- configuration guidance
- release notes
- public issue templates
- support and contact information

This repository does **not** contain the private agent implementation.

---

## What the Treasurer Agent Does

The Treasurer Agent is intended to help automate routine nonprofit finance operations, including:

- reviewing transactions
- assisting with bookkeeping categorization
- preparing reconciliation summaries
- organizing receipts and supporting documents
- generating accountant-facing reports
- drafting finance-related emails
- checking for missing records
- supporting month-end and year-end workflows

The agent is not a replacement for a licensed accountant, attorney, auditor, or tax professional.

---

## Local-First Design

The Treasurer Agent is designed to run locally or inside infrastructure controlled by the user.

By default:

- financial data remains in the user-controlled environment;
- Hush Line does not automatically receive transaction-level accounting data;
- integrations are configured by the user;
- outputs should be reviewed before being relied upon.

Depending on configuration, the agent may connect to third-party services such as accounting software, banking APIs, email providers, GitHub, or AI model providers.

---

## Public Repo / Private Code Model

This project uses a split-repository model:

| Repository | Visibility | Purpose |
|---|---:|---|
| Public repository | Public | Documentation, policies, legal terms, support info, transparency |
| Agent implementation repository | Private | Source code, workflows, secrets handling, integrations, internal logic |

This structure allows Hush Line to publish user-facing terms and operational documentation while keeping sensitive implementation details private.

---

## Important Limitations

The Treasurer Agent may produce incorrect, incomplete, or misleading outputs.

Users must independently verify:

- bookkeeping entries
- reconciliations
- account balances
- reports
- tax-related materials
- regulatory filings
- accountant communications
- automated actions

The agent does not provide legal, tax, accounting, audit, fiduciary, or investment advice.

---

## Security Expectations

Users are responsible for securing the environment where the agent runs.

Recommended controls include:

- full-disk encryption
- encrypted backups
- MFA on financial accounts
- least-privilege API credentials
- separate service accounts where possible
- restricted filesystem permissions
- audit logging
- routine software updates
- secret scanning
- human review before external communications or financial submissions

Do not commit secrets, credentials, tokens, bank exports, accounting files, or financial records to this public repository.

---

## Privacy

The Treasurer Agent is intended to be local-first.

However, depending on user configuration, data may be sent to third-party services such as:

- accounting platforms
- banking APIs
- email providers
- cloud storage providers
- AI model providers
- notification systems

See [`PRIVACY.md`](./PRIVACY.md) for the full privacy policy.

---

## License

Use of the Treasurer Agent is governed by the project EULA.

See [`EULA.md`](./EULA.md).

---

## Support

For questions, support, or security concerns, contact Hush Line:

https://hushline.app

---

## Security Reports

Please do not publicly disclose security vulnerabilities.

If you believe you have found a security issue, contact Hush Line privately through the support channel listed above.

---

## Disclaimer

The Treasurer Agent is provided as a workflow automation tool.

It is not professional financial advice, legal advice, tax advice, audit advice, or fiduciary service.

Use at your own risk.
