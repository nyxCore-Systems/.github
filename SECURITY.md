# Security policy

nyxCore takes security seriously across every product in the roster. If you
believe you have discovered a vulnerability, please follow the process
below — not a public issue.

## Reporting a vulnerability

Email **[hello@nyxcore.cloud](mailto:hello@nyxcore.cloud)** with the subject
line `[SECURITY]`. The inbox routes through our own docker-mailserver on
Hetzner Frankfurt — no third-party email provider sees your report.

Please include:

- A description of the issue and the product(s) affected.
- Steps to reproduce.
- A proof-of-concept if you have one.
- Contact details so we can follow up.

## What to expect

| Step | Target |
|---|---|
| Acknowledgement of receipt | within 2 business days |
| Initial severity assessment + proposed timeline | within 5 business days |
| Coordinated disclosure for high / critical issues | within 30 days |
| Coordinated disclosure for medium / low issues | within 90 days |
| Credit in the release notes (opt-in) | at disclosure time |

## Scope

In scope:

- All repositories under the [nyxCore-Systems](https://github.com/nyxCore-Systems)
  organisation.
- The nyxCore dashboard served at [nyxcore.cloud](https://nyxcore.cloud) and
  [core.nyxcore.cloud](https://core.nyxcore.cloud), including tenant
  isolation (PostgreSQL RLS), the BYOK key vault (AES-256-GCM), audit logs,
  and the multi-provider LLM routing layer.
- All product landings at `*.nyxcore.cloud`.
- The production runtime on Hetzner Frankfurt — Traefik, Postgres 16,
  Redis 7, our Prometheus / Loki / Grafana stack.

Out of scope:

- Third-party services we route through (Anthropic, OpenAI, Google, Ollama,
  Resend, Supabase). Report those to the respective vendor.
- Denial-of-service attempts or load-testing against production endpoints.
- Physical attacks or social engineering of our team.
- Clickjacking, self-XSS, or issues that require user interaction the user
  would not reasonably perform.

## Persona review

Every advisory runs through **Nemesis** (vulnerability detection),
**Aletheia** (code → regulation mapping), and **Themis** (compliance,
GDPR / ISO 27001). Nemesis drafts the disclosure text; Themis signs off
before release. The full pantheon is at
[landingpage.nyxcore.cloud#pantheon](https://landingpage.nyxcore.cloud/#pantheon).

## Preferred language

Reports in English or German are easiest for us to triage. Portuguese works
too; expect an extra day for the translation round-trip.

---

<sub>© 2026 nyxCore Systems · Responsible disclosure, coordinated release.</sub>
