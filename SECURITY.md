# Security Policy

## Supported Versions

| Plugin | Version | Supported |
|---|---|---|
| expo-app-design | latest | YES |
| upgrading-expo | latest | YES |
| expo-deployment | latest | YES |
| Any version < 1.0 | -- | NO |

## Reporting a Vulnerability

**Do NOT open a public GitHub issue for security vulnerabilities.**

Report security issues privately to the Expo security team:

- **Email:** security@expo.dev
- **Expected response time:** 48 hours
- **Disclosure policy:** We follow coordinated disclosure. Please allow 90 days before public disclosure.

## Skill Integrity Guidance

All official Expo skills in this repository are maintained by verified contributors.
Before installing **any** third-party or community skill, review the SKILL.md file for:

- Undeclared external network calls or URL fetching
- Broad or unscoped filesystem access patterns
- Instructions that override or suppress agent safety guidance
- Requests to exfiltrate credentials, tokens, or environment variables

## Supply Chain Risk Context

AI agent skill repositories are an emerging supply chain attack surface. Researchers have
documented malicious skill packages using typosquatting, prompt injection payloads, and
credential-harvesting instructions in community skill ecosystems (ref: Antiy CERT ClawHub
analysis, 2026; OWASP Top 10 for Agentic Applications 2026, ASI04).

This repository mitigates that risk through:
- Verified contributor requirements on the main branch
- SHA-256 checksums in marketplace.json (see schema)
- Trust tier classification (official / verified / community)
- Permission scope declarations in plugin.json manifests

## Known Security Advisories

No active advisories. See GitHub Security Advisories for history.
