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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The Technical University of Denmark (DTU) is a technical university in Kongens Lyngby, Denmark. DTU operates no central developer portal and publishes no OpenAPI-described public REST API of its own — `api.dtu.dk` and `developer.dtu.dk` do not resolve. Its two clearly institution-operated machine-readable surfaces are its identity federation (a DTU-run SAML 2.0 / WS-Federation / OpenID Connect token service at `sts.ait.dtu.dk`, registered in the Danish national federation WAYF and in eduGAIN) and the Global Wind Atlas OGC Web Processing Service, whose GetCapabilities document names DTU Wind Energy as the service provider with a `dtu.dk` contact. DTU Data (`data.dtu.dk`) is a Figshare tenant and DTU Orbit (`orbit.dtu.dk`) is an Elsevier Pure deployment: both are recorded here as tenant relationships, not as DTU contracts.

APIs.json: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/apis.yml

Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=dtu-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Technical University
- Denmark
- Europe
- Identity Federation
- Research Data
- Library
- Course Catalog
- Wind Energy

## APIs

Every entry carries an `x-operator` recording **who runs the thing** — for a university that is
almost never the same answer as who the surface is named after.

**Institution-operated**

- **DTU Identity Federation (SAML 2.0 / WS-Federation / OpenID Connect)** — DTU's own security token
  service at `sts.ait.dtu.dk`. Signed SAML metadata and an OIDC discovery document are served openly and
  unauthenticated. IdP entityID `http://sts.ait.dtu.dk/adfs/services/trust`, registered in WAYF and eduGAIN
  with `schacHomeOrganization: dtu.dk`.
  Metadata: https://sts.ait.dtu.dk/FederationMetadata/2007-06/FederationMetadata.xml —
  Discovery: https://sts.ait.dtu.dk/adfs/.well-known/openid-configuration
- **Global Wind Atlas Web Processing Service** — OGC WPS 1.0.0, eight processes, fees "None".
  `ows:ProviderName` is DTU Wind Energy, contact `neda@dtu.dk`, Risø Campus, Roskilde.
  Capabilities: https://wps.globalwindatlas.info/?service=WPS&request=GetCapabilities —
  Docs: https://wasp.dtu.dk/wind-atlases/global-wind-atlas
- **DTU Findit** — DTU Library discovery on DTU's own host (open-source Blacklight). Publishes an
  OpenSearch 1.1 description; catalog responses sit behind a verification interstitial for non-browser
  clients. Descriptor: https://findit.dtu.dk/en/catalog/opensearch.xml
- **DTU course base** — `kurser.dtu.dk`. DTU-operated, but every path returns a 371-byte forced-sign-in
  shell. Real surface, authentication gated, no public data. Portal: https://kurser.dtu.dk/

**Tenant — DTU's data, a vendor's contract**

- **DTU Data (Figshare tenant)** — DTU's institutional research data repository, Figshare institution id
  379. The API serving it is `api.figshare.com/v2`, a generic host every Figshare customer shares, so no
  OpenAPI is stored here for it. Portal: https://data.dtu.dk/ — Docs: https://docs.figshare.com/
- **DTU Orbit (Elsevier Pure tenant)** — research information database on DTU's own host, deployed on
  Elsevier Pure. Portal behind a Cloudflare bot challenge; Pure's OAI-PMH and web-service paths error.
  Portal: https://orbit.dtu.dk/
- **DTU Learn (D2L Brightspace tenant)** — the LMS. Brightspace's LTI certification is D2L's, not DTU's,
  and DTU publishes no LTI platform configuration of its own. Portal: https://learn.dtu.dk/

## Identity, Authentication and Conformance

- [authentication/dtu-authentication.yml](authentication/dtu-authentication.yml)
- [conformance/dtu-conformance.yml](conformance/dtu-conformance.yml) — one evidenced `education`-regime
  domain-standard hit: **saml**. The other eleven are recorded as probed misses with status codes.

## Plans

- [plans/dtu-plans-pricing.yml](plans/dtu-plans-pricing.yml)

## Rate Limits

- [rate-limits/dtu-rate-limits.yml](rate-limits/dtu-rate-limits.yml)

## FinOps

- [finops/dtu-finops.yml](finops/dtu-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.dtu.dk/english
- IdentityFederation: https://sts.ait.dtu.dk/FederationMetadata/2007-06/FederationMetadata.xml
- ResearchRepository: https://data.dtu.dk/
- LibraryCatalog: https://findit.dtu.dk/
- CourseCatalog: https://kurser.dtu.dk/
- ResearchComputing: https://www.hpc.dtu.dk/
- AIPolicy: https://www.ai.dtu.dk/rules/
- AITooling: https://www.ai.dtu.dk/
- GitHubOrganization: https://github.com/dtudk
- GitHub: https://github.com/DTUWindEnergy
- LinkedIn: https://www.linkedin.com/school/technical-university-of-denmark/
- PrivacyPolicy: https://www.dtu.dk/english/about/strategy-policy/policies/privacy-policy
- Blog: https://www.dtu.dk/english/news/all-news

## Notes

- Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles **who operates a
  surface** before any contract is saved.
- **Five Figshare OpenAPI contracts and the 17 artifacts derived from them were removed from this repo.**
  `api.figshare.com` is a generic vendor host claimed by four other institutions in this cohort; the
  contract is Figshare's engineering and belongs in Figshare's own repo, not DTU's. The tenant
  *relationship* is kept, because it is a real institutional fact.
- Two genuinely institution-operated machine-readable surfaces the June 2026 profile missed were found
  and verified: DTU's own SAML/OIDC token service, and the Global Wind Atlas OGC WPS.
- No OAI-PMH endpoint on a DTU-operated host responded (`orbit.dtu.dk/ws/oai?verb=Identify` → 500,
  `findit.dtu.dk/oai` → 404). No open data portal exists.
- DTU's IdP is Microsoft AD FS, not Shibboleth — the earlier profile's "Shibboleth/OCES" note was wrong.
- No endpoints were fabricated. Gated, challenged and erroring interfaces are documented with their
  status codes. A 403 bot challenge grades **live**, not dead.

## Maintainers

- Kin Lane — kin@apievangelist.com
