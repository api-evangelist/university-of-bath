# University of Bath (university-of-bath)

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

The University of Bath is a public research university in Bath, United Kingdom, ranked #150 in the QS World University Rankings 2025. This repository catalogs the institution's public, machine-readable developer/API footprint as an APIs.json provider profile. That footprint is scholarly-metadata oriented — an Elsevier Pure research portal with an OAI-PMH interface, an EPrints 3.4 Research Data Archive (OAI-PMH plus REST/feeds), and an Ex Libris Alma/Primo library discovery platform — rather than a commercial developer program.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-bath/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-bath-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, United Kingdom, Research, Open Data, Library, Metadata

## APIs

- **Research Portal (Pure) OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the University of Bath Open Access Repository (Elsevier Pure). Base URL `https://purehost.bath.ac.uk/ws/oai`. Docs: https://www.bath.ac.uk/guides/overview-of-pure/
- **Research Data Archive OAI-PMH** — OAI-PMH 2.0 endpoint for the EPrints 3.4 Research Data Archive. Base URL `https://researchdata.bath.ac.uk/cgi/oai2`. Docs: https://researchdata.bath.ac.uk/
- **Research Data Archive REST/Feeds** — EPrints REST/XML interface and RSS/Atom feeds. Base URL `https://researchdata.bath.ac.uk/rest`. Docs: https://researchdata.bath.ac.uk/
- **Library Discovery (Ex Libris Primo)** — Alma/Primo library catalogue and discovery; programmatic Primo APIs require an Ex Libris key. Front end `https://bath.primo.exlibrisgroup.com/`. Docs: https://www.bath.ac.uk/guides/using-the-library-catalogue/
- **Azure API Management Developer Portal (non-production)** — Azure APIM developer portal; only a non-production "test" instance is publicly reachable, with no documented production APIs. https://portal.apim.test.bath.ac.uk/

## Plans

See [plans/university-of-bath-plans-pricing.yml](plans/university-of-bath-plans-pricing.yml).

## Rate Limits

See [rate-limits/university-of-bath-rate-limits.yml](rate-limits/university-of-bath-rate-limits.yml).

## FinOps

See [finops/university-of-bath-finops.yml](finops/university-of-bath-finops.yml).

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.bath.ac.uk/
- GitHub: https://github.com/uniofbathdmc
- LinkedIn: https://www.linkedin.com/school/university-of-bath/
- Developer Portal: https://portal.apim.test.bath.ac.uk/ (non-production)
- Plans: plans/university-of-bath-plans-pricing.yml
- Rate Limits: rate-limits/university-of-bath-rate-limits.yml
- FinOps: finops/university-of-bath-finops.yml
- Review: review.yml

## Notes

All endpoints were probed live on 2026-06-03; no APIs or endpoints were fabricated. The Pure OAI-PMH interface is confirmed via the Identify verb (Pure 5.33.3-3). The EPrints Research Data Archive OAI-PMH and REST paths both resolve (HTTP 200). The publicly reachable Azure APIM portal is a "test" (non-production) environment, so it is listed for transparency only with no production endpoints claimed. The `researchportal.bath.ac.uk/ws/oai` path returned HTTP 500 and was excluded in favor of the working `purehost.bath.ac.uk` endpoint. The LinkedIn page returns HTTP 999 (LinkedIn anti-bot), but the school URL is valid.

## Maintainers

- Kin Lane — kin@apievangelist.com
