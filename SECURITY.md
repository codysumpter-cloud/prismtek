# Security Policy

## Reporting a vulnerability

Please **do not open a public issue** for a vulnerability, live credential, exploit chain, or private user information.

Email **prismtek@prismtek.dev** with the subject `Prismtek security report`. Include the affected public project and version, a concise impact summary, and safe reproduction steps. Do not send real player passwords or other users' private data.

We will review reports, but do not promise a fixed response time or a bug bounty.

## Supported versions

Only explicitly published, maintained project releases are candidates for security fixes. This repository currently contains documentation and project plans; **no installable addon release has been published here**.

## Secrets and API design

- Never commit or publish API keys, tokens, private keys, player credentials, or service account files.
- Do not put service API credentials in downloaded addons, browser bundles, mobile clients, or screenshots.
- Use an approved, access-controlled server-side integration when external credentials are required, and follow the API provider's restrictions.
- A `.gitignore` file is not a security boundary. Review every public change for secrets and third-party material before merging.
- If a real secret is exposed, revoke/rotate it and investigate exposure; deleting a file or commit alone is insufficient.

See [docs/PUBLISHING.md](docs/PUBLISHING.md).
