# Security Policy

This policy applies to all public repositories in this organization unless a
repository ships its own `SECURITY.md`.

## Reporting a Vulnerability

**Do not open a public issue for security vulnerabilities.**

Report privately via either:

1. **GitHub Private Vulnerability Reporting** (preferred) — open a private
   advisory on the affected repository's **Security** tab.
2. **Email** — `heznpc@gmail.com` as fallback when private advisories are
   not enabled on a repository.

Please include:
- Affected repository and (if known) version / commit SHA
- Steps to reproduce or proof-of-concept
- Impact assessment (data exposure, RCE, DoS, etc.)
- Suggested fix if you have one

## Response SLA

| Stage | Target |
|---|---|
| Acknowledgement | 48 hours |
| Initial assessment + severity rating | 5 business days |
| Coordinated disclosure | 90 days from acknowledgement (expedited for high-severity issues with active exploitation) |

We follow coordinated disclosure. Once a fix ships and users have a
reasonable update window, we publish a GitHub Security Advisory and — for
qualifying issues — request a CVE.

## Scope

**In scope**
- Source code in active (non-archived) repositories
- Build, CI, and release pipelines
- Default configurations published in our starters / templates

**Out of scope**
- Archived repositories (clearly marked in repo description) — report to
  the project's last active maintainer instead
- Vulnerabilities in third-party dependencies — please report directly to
  the upstream maintainer. We mirror the fix once a patched version is
  available.
- Social-engineering attempts against maintainers
- Denial-of-service against public demo / preview deployments
- Issues that require physical access to the maintainer's machine

## Public Disclosure

After a patch is released and the update window has elapsed, we publish:
- A GitHub Security Advisory on the affected repository
- A CVE identifier where applicable
- Credit to the reporter (or anonymous credit on request)

If you reported a vulnerability and have not heard back within the
acknowledgement SLA, please re-send via the fallback channel.
