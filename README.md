# Technical University of Denmark (dtu)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
