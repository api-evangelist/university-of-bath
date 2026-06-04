# University of Bath (university-of-bath)

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
