# Technical University of Denmark (dtu)

The Technical University of Denmark (DTU) is a leading engineering and science university in Kongens Lyngby, Denmark, ranked #109 in the QS World University Rankings 2025. Its public developer/API footprint is research- and metadata-oriented: the DTU Data repository exposes the open Figshare REST API, and DTU Orbit runs on Elsevier Pure. DTU also maintains a public GitHub organization for affiliated open-source software. There is no consolidated institution-wide public developer portal.

APIs.json: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/apis.yml

Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=dtu-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research Data
- Open Data
- Denmark
- Europe

## APIs

- **DTU Data (Figshare API)** — DTU's institutional research data repository on Figshare; public datasets and metadata via the Figshare REST API v2 scoped to DTU institution id 379. Docs: https://docs.figshare.com/ — Portal: https://data.dtu.dk/
- **DTU Orbit Research Database (Pure)** — DTU's Elsevier Pure research information database (publications, projects, profiles). Public web portal is browsable; Pure OAI/web-service endpoints are gated/erroring on the public host. Docs: https://www.bibliotek.dtu.dk/en/about-and-contact/open-science/open-science-dtu-orbit — Portal: https://orbit.dtu.dk/

## Plans

- [plans/dtu-plans-pricing.yml](plans/dtu-plans-pricing.yml)

## Rate Limits

- [rate-limits/dtu-rate-limits.yml](rate-limits/dtu-rate-limits.yml)

## FinOps

- [finops/dtu-finops.yml](finops/dtu-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.dtu.dk/english
- GitHub: https://github.com/dtudk
- LinkedIn: https://www.linkedin.com/school/technical-university-of-denmark/
- Authentication: https://auth.dtu.dk/

## Notes

- All cataloged URLs were probed on 2026-06-03. The Figshare-backed DTU Data API returned live JSON (HTTP 200).
- DTU Orbit's public Pure OAI/web-service endpoint redirected to an error page (HTTP 500) and is not openly documented or self-service; it is cataloged as a portal, not a usable API.
- No dedicated `developer.dtu.dk` portal exists. Identity/SSO is handled via DTU's federated authentication (Shibboleth/OCES).
- No endpoints were fabricated; gated and erroring interfaces are documented honestly.

## Maintainers

- Kin Lane — kin@apievangelist.com
