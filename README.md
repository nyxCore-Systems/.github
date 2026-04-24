# nyxCore Systems · organisation profile

This repository holds the files GitHub surfaces at the organisation level —
the profile page rendered on [github.com/nyxCore-Systems](https://github.com/nyxCore-Systems),
the responsible-disclosure policy, and shared contribution defaults.

## Layout

```
.
├── README.md                 ← this file (meta-README)
├── SECURITY.md               ← responsible-disclosure channel for every product
└── profile/
    └── README.md             ← rendered as the org front page
```

## Editing the profile

The profile page is the surface visitors see first. Edits should:

1. **Stay in sync with [landingpage.nyxcore.cloud](https://landingpage.nyxcore.cloud).**
   The ecosystem list, team roles, pantheon counts, and savings numbers on
   the README must not drift from the ones on the landing page. If a product
   moves between integration categories, both places change in one commit.
2. **Run through an Aristaeus + Metis review before merge.**
   No marketing softener, numbers carry weight. Any "honest positioning"
   copy goes through the Ipcha rulebook —
   [`IPCHA_DISCLOSURES.md`](https://github.com/nyxCore-Systems/nyxcore-landingpage/blob/main/docs/IPCHA_DISCLOSURES.md)
   — before shipping.
3. **Pull live numbers from the nyxCore MCP where possible.**
   Persona-run counts, tRPC router count, savings ranges — if a number can
   be derived from the knowledge base it should not be hand-edited into the
   README.

## Related repositories

- [`nyxcore-landingpage`](https://github.com/nyxCore-Systems/nyxcore-landingpage)
  — the ecosystem landing + every product sub-site at `*.nyxcore.cloud`.
- [`nyxcore-systems`](https://github.com/nyxCore-Systems/nyxcore-systems) —
  the dashboard, the orchestration brain. Served at
  [core.nyxcore.cloud](https://core.nyxcore.cloud).
- The full product roster (18 repositories) is listed on the
  [organisation page](https://github.com/nyxCore-Systems).

## Licence

All rights reserved on the marketing copy in this repository. Source code
of the individual products lives in their own repositories with their own
licences (MIT, Apache-2.0, tiered-commercial, etc.) — see each product's
own `LICENSE` file.

---

<sub>© 2026 nyxCore Systems (GmbH in Gründung) · Feldstrasse 26 · 21335 Lüneburg · <a href="mailto:hello@nyxcore.cloud">hello@nyxcore.cloud</a></sub>
