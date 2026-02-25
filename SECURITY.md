# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in Argus, please report it responsibly.

**Do not open a public GitHub issue for security vulnerabilities.**

Instead, please email: **security@salimmohamed.dev**

Include:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

## Response Timeline

- **Acknowledgment:** Within 48 hours
- **Initial assessment:** Within 1 week
- **Fix timeline:** Depends on severity, typically within 2 weeks for critical issues

## Scope

Argus processes external API data from Polymarket and The Graph. It does not handle user authentication or store personally identifiable information (PII).

Security concerns most relevant to this project:
- API key exposure
- Data injection through external API responses
- Convex function authorization
- Environment variable handling

## Supported Versions

| Version | Supported |
|---------|-----------|
| 0.2.x   | Yes       |
| < 0.2   | No        |
