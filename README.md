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

The University of Bath is a public research university in Bath, United Kingdom, and a member of the Russell Group. This repository catalogs the institution's public, machine-readable footprint as an APIs.json provider profile, with **who operates each surface** recorded alongside it.

Bath runs no public developer program. A crawl of its 21,530-URL sitemap on 2026-08-30 found no developer portal, no API reference and no published OpenAPI anywhere under bath.ac.uk. Its one genuinely institution-operated programmable surface is the **Research Data Archive** at `researchdata.bath.ac.uk` — EPrints 3.4.7 on the University's own infrastructure (138.38.44.144) — serving OAI-PMH 2.0, an EPrints REST/XML interface, and DataCite kernel-4 records with ORCID iDs and DOIs under Bath's own `10.15125` prefix.

Everything else that looks like a Bath API is a **vendor contract under a Bath hostname**: `purehost.bath.ac.uk` and `researchportal.bath.ac.uk` both CNAME to `bath-prod.elsevierpure.com` (Elsevier Pure); the catalogue is an Ex Libris Alma/Primo tenancy; `library.bath.ac.uk` is Springshare LibGuides; `status.bath.ac.uk` is Better Stack. Those are recorded as **tenant** relationships — real institutional facts — and their contracts are deliberately not stored here.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-bath/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-bath-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

University, Higher Education, Education, United Kingdom, Russell Group, Research Data, Research Repository, Open Data, Library, OAI-PMH, Metadata, Research Computing

## APIs

Each surface carries an operator. `institution` means Bath runs the thing the contract describes; `tenant` means Bath's data and Bath's deployment on someone else's platform, under someone else's contract.

**institution**

- **Research Data Archive OAI-PMH** — OAI-PMH 2.0 for the EPrints 3.4.7 Research Data Archive, on Bath's own infrastructure. Seven metadata prefixes: `didl`, `mets`, `oai_bibl`, `oai_datacite`, `oai_dc`, `rdf`, `uketd_dc`. Base URL `https://researchdata.bath.ac.uk/cgi/oai2`. Docs: https://researchdata.bath.ac.uk/
- **Research Data Archive REST/XML** — EPrints REST interface exposing the `eprint`, `user` and `subject` datasets. Base URL `https://researchdata.bath.ac.uk/rest`. Docs: https://researchdata.bath.ac.uk/

**tenant**

- **Research Portal (Elsevier Pure) Web Service** — the Pure Web Service under a Bath hostname. Documentation returns 200; `/ws/api/524/openapi.yaml` returns 401. The contract is titled "Pure API" with contact `pure-support@elsevier.com` and a relative server of `/ws/api` — nine other institutions in this cohort shipped the identical document as their own. Base URL `https://purehost.bath.ac.uk/ws/api`.
- **Research Portal (Elsevier Pure) OAI-PMH** — OAI-PMH 2.0 with the OpenAIRE CERIF 1.2 profile. Live but defective: `ListMetadataFormats` and `ListRecords` return 200 while the mandatory `Identify` verb returns an Elsevier HTML 500. Base URL `https://purehost.bath.ac.uk/ws/oai`.
- **Library Discovery (Ex Libris Alma/Primo)** — the Bath view (`vid=44BAT_INST:NDE`) on Ex Libris's host; programmatic Primo/Alma APIs need an Ex Libris key. Front end `https://bath.primo.exlibrisgroup.com/`. Docs: https://www.bath.ac.uk/guides/using-the-library-catalogue/

**not recorded as a surface**

- `portal.apim.test.bath.ac.uk` — an Azure API Management **test** instance. A non-production host is not a surface, so it is no longer listed as one.

## Conformance

Domain standards confirmed against live responses, not against prose claims — see [conformance/university-of-bath-conformance.yml](conformance/university-of-bath-conformance.yml): **oai-pmh**, **datacite** and **orcid**, all on the institution-operated Research Data Archive. Bath's UK Access Management Federation / eduGAIN entry could not be retrieved (`idp.bath.ac.uk` did not answer on 443 from this network), so `shibboleth` and `saml` are recorded as unconfirmed rather than claimed.

## Plans

See [plans/university-of-bath-plans-pricing.yml](plans/university-of-bath-plans-pricing.yml).

## Rate Limits

See [rate-limits/university-of-bath-rate-limits.yml](rate-limits/university-of-bath-rate-limits.yml).

## FinOps

See [finops/university-of-bath-finops.yml](finops/university-of-bath-finops.yml).

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.bath.ac.uk/
- GitHub Organization: https://github.com/uniofbathdmc
- LinkedIn: https://www.linkedin.com/school/university-of-bath/
- Research Repository: https://researchdata.bath.ac.uk/ · https://researchportal.bath.ac.uk/
- Library Catalog: https://library.bath.ac.uk/home
- Course Catalog: https://www.bath.ac.uk/courses/
- Open Data: https://www.bath.ac.uk/topics/open-research/
- Research Computing: https://www.bath.ac.uk/professional-services/research-computing/
- AI Policy: https://www.bath.ac.uk/guides/student-guidance-on-uploading-documents-to-genai-tools-or-third-party-websites/
- AI Tooling: https://www.bath.ac.uk/announcements/support-for-students-to-use-genai-tools-effectively-and-responsibly/
- Privacy Policy: https://www.bath.ac.uk/legal-information/data-protection-and-privacy-statement-summary/
- Status: https://status.bath.ac.uk/
- ROR: https://ror.org/002h8g185
- Conformance: conformance/university-of-bath-conformance.yml
- Plans: plans/university-of-bath-plans-pricing.yml
- Rate Limits: rate-limits/university-of-bath-rate-limits.yml
- FinOps: finops/university-of-bath-finops.yml
- Review: review.yml

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles **who operates a surface** before saving any contract.

The June 2026 profile credited this institution with 21 OpenAPI definitions, 43 Postman/OpenCollection files, 5 JSON Schemas, 5 JSON Structures, 5 examples, 2 rulesets, a vocabulary, a JSON-LD context, an authentication profile, an agentic-access profile covering 663 operations, and a capability map. Every one of them was derived from a **single Elsevier Pure contract** — `info.title: Pure API`, `info.contact: pure-support@elsevier.com`, `servers: [/ws/api]` — that nine other institutions in this cohort ship verbatim. **88 files were removed.** The Pure deployment itself was kept and correctly relabelled as a tenant relationship: the data is Bath's, the engineering is Elsevier's.

Everything below was probed live on 2026-08-30; nothing was fabricated.

- `researchdata.bath.ac.uk` resolves via `researchdata-1.bath.ac.uk` to **138.38.44.144**, inside Bath's own address space — the operator verdict here is institution, and it is the only one.
- `purehost.bath.ac.uk` and `researchportal.bath.ac.uk` both CNAME to `bath-prod.elsevierpure.com` → `eu.prod.elsevierpure.com`. A hostname under `bath.ac.uk` is not evidence of institutional operation, and this repo is a worked example of why.
- `purehost.bath.ac.uk/ws/oai?verb=Identify` now returns **HTTP 500**. The June profile recorded this exact verb as confirmed live (Pure 5.33.3-3). Other verbs still answer 200.
- `status.bath.ac.uk/api/v2/status.json` returns 200 with `content-type: text/html` and the same byte length as the homepage — a soft-404 SPA shell, not a status API. Not credited.
- `www.bath.ac.uk/llms.txt` and `/.well-known/security.txt` both 404. `www.bath.ac.uk/catalogues/` redirects to CAS at `auth.bath.ac.uk`; `samis.bath.ac.uk` redirects to Microsoft Entra ID. `idp.bath.ac.uk` did not answer on 443 across two attempts.
- The LinkedIn page returns HTTP 999 (LinkedIn anti-bot); the school URL is valid.

A university that publishes almost nothing, and says so, is a correct profile — not a failed one. This one's score should fall, because the previous number was Elsevier's.

## Maintainers

- Kin Lane — kin@apievangelist.com
