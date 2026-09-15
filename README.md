# Aero Browser

A Chromium-based privacy browser. No ads. No crypto. No telemetry. Fingerprint resistance on by default. Built by one 14-year-old kernel contributor from Hyderabad, growing into a small founding team.

## Status

Founding phase. v0.1 targets a working Linux build with Google telemetry stripped, uBlock Origin built in, and DNS-over-HTTPS enabled by default.

**Maintainer on exam break: Sept 28 – Oct 9, 2026.** Issues and PRs will be triaged starting Oct 10. The project is not abandoned.

## What Aero is

A fork of [ungoogled-chromium](https://github.com/ungoogled-software/ungoogled-chromium) with a minimal patch stack, built around three principles:

- **Zero ads.** Not "acceptable ads," not "replaced ads," not "partner ads." Zero.
- **Zero telemetry.** No analytics, no crash reporting, no usage pings. Verifiable.
- **Zero compromise.** No crypto wallet, no VPN upsell, no affiliate links, no AI assistant that phones home.

## What Aero is not

- Not a Brave clone. Brave is a company with investors and a crypto business model. Aero is a project with no business model.
- Not Tor Browser. Tor is for high-risk anonymity. Aero is for everyday privacy.
- Not finished. It's barely started. Be patient.

## Founding lanes

| Lane | Owner | Status |
|------|-------|--------|
| 1. Build & CI | [open] | Recruiting |
| 2. Chromium core patches | [open] | Recruiting |
| 3. Features (shields, settings) | [open] | Recruiting |
| 4. Docs, tests | [open] | Recruiting |
| 5. Privacy research | [open] | Recruiting |

Lane 6 (packaging) and Lane 7 (upstream sync) are deferred until v0.1 ships.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Bug fixes and docs go straight to PR. New features need an issue first. Async-first — this project is maintained around a school schedule.

## Contributors

- [@builtbyashwin](https://github.com/builtbyashwin) — maintainer, build/CI, upstream sync
- [@Arman16-1998](https://github.com/Arman16-1998) — docs, privacy research

## License

GPL-3.0. If you fork Aero and add telemetry, you have to publish that fact. That's the point.
