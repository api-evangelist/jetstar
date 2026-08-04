# Jetstar (jetstar)

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

Jetstar Airways Pty Limited (ABN 33 069 720 243) is the Melbourne-based low-cost carrier of the Qantas Group and, with Virgin Australia, one half of the Australian domestic duopoly. The Jetstar Group flies as Jetstar Airways (JQ) and Jetstar Japan (GK); Jetstar Asia (3K) flew its last service on 31 July 2025. Jetstar sits at the direct-distribution end of the Australian travel chain: it sells through jetstar.com, through the Jetstar Agent Hub, through seven GDSs, and through a partner channel it calls, literally, the Jetstar API. That API is not a public developer product and it is not IATA NDC — it is the Navitaire New Skies SOAP web service (NSK 4.6) hosted on the vendor's own domain at jqapi.navitaire.com, with documentation, registration and downloads behind a login at apiblog.jetstar.com. There is no public developer portal, no OpenAPI or WSDL published, no self-serve signup and no bulk export operation.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jetstar/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jetstar/refs/heads/main/apis.yml)

## Tags

- Travel
- Australia
- Aviation
- Airline
- Low Cost Carrier
- Distribution
- Booking
- GDS
- Corporate Travel
- Qantas Group

## Timestamps

- **Created:** 2026-07-28
- **Modified:** 2026-07-28

## APIs

### Jetstar API

The Jetstar API is Jetstar's direct-connect distribution channel for Registered Travel Agents and partners. It is a Navitaire New Skies (NSK) SOAP / WCF web service, not a REST product and not IATA NDC. Jetstar's own partner FAQ publishes the environments as NSK 4.6 with production at `https://jqapi.navitaire.com` and test at `https://soapapir4y.test.jq.navitaire.com`, and documents WCF services such as `UtilitiesManager.svc` alongside session-signature authentication. Operations named in Jetstar's published partner documentation include `GetAvailability`, `GetTripAvailabilityWithSSR`, `PriceItinerary`, `GetItineraryPrice`, `GetSSRAvailability`, `GetStationList`, `AddPaymentToBooking`, `BookingCommit`, `GetBooking` and `UpdatePassengers`. Documentation, registration, an API Products page and a Download Centre live at apiblog.jetstar.com behind a partner login; no OpenAPI, WSDL or machine-readable contract is published publicly.

- **Human URL:** [https://apiblog.jetstar.com/](https://apiblog.jetstar.com/)
- **Base URL:** `https://jqapi.navitaire.com`

#### Tags

- Airline
- Distribution
- Booking
- SOAP
- Navitaire
- New Skies
- Travel Agents
- Ancillaries

#### Properties

- [Portal](https://apiblog.jetstar.com/)
- [Documentation](https://apiblog.jetstar.com/api-documentation/)
- [FAQ](https://apiblog.jetstar.com/faq/)
- [Signup](https://apiblog.jetstar.com/api-registration/)
- [Documentation](https://apiblog.jetstar.com/api-products/)
- [Downloads](https://apiblog.jetstar.com/downloads/)
- [Blog](https://apiblog.jetstar.com/blog/)
- [Authentication](https://apiblog.jetstar.com/login/)
- [Support](mailto:apisupport@jetstar.com)
- [Terms Of Service](https://www.jetstar.com/us/en/travel-agents/terms-and-conditions)

## Common Properties

- [Website](https://www.jetstar.com/)
- [Portal](https://apiblog.jetstar.com/)
- [Documentation](https://www.jetstar.com/us/en/travel-agents/information-centre/jetstar-api)
- [Getting Started](https://www.jetstar.com/us/en/travel-agents/why-become-a-registered-travel-agent-with-jetstar)
- [Signup](https://www.jetstar.com/us/en/travel-agents)
- [Terms Of Service](https://www.jetstar.com/us/en/travel-agents/terms-and-conditions)
- [Privacy](https://www.jetstar.com/au/en/privacy-policy)
- [Support](mailto:apisupport@jetstar.com)
- [Support](mailto:sales@jetstar.com)
- [Documentation](https://www.jetstar.com/us/en/travel-agents/information-centre/bsp-settlement)
- [Documentation](https://www.jetstar.com/us/en/travel-agents/bsp-payment-changes)
- [Documentation](https://www.jetstar.com/au/en/travel-agents/remuneration)
- [FAQ](https://www.jetstar.com/_/media/files/qantas-group/qantas-group-081-faqs.pdf)
- [GitHub Organization](https://github.com/JetstarAirways)
- [LinkedIn](https://www.linkedin.com/company/jetstar-airways)
- [Blog](https://newsroom.jetstar.com/)

## Switching Cost

Full evidence is recorded in [review.yml](review.yml). Summary:

| Dimension | Finding |
| --- | --- |
| Interface shape | `proprietary-documented` — Navitaire New Skies (NSK 4.6) SOAP/WCF, vendor-defined, no standard reference found |
| Second source | `no-alternative` for Jetstar's own seat inventory |
| Exit path | `export-on-request` — no bulk export operation published; per-PNR retrieval only |
| Identifier portability | IATA designators JQ/GK, PNR record locators, IATA station codes, IATA agency number, QF 081 ticket stock, IATA SSR + Reg 830d fields; Navitaire session signatures and product/fare-basis codes are not portable |
| Contractual lock-in | Three authorised booking facilities only (API, GDS, Agent Hub); booking on Jetstar.com for commercial purposes breaches the Travel Agent T&Cs |
| Distribution model | `gds-intermediated` in the enum, but in practice a hybrid: direct Navitaire API plus a partial GDS overlay with incomplete fare content |
| NDC posture | No IATA NDC. No NDC endpoint, no NDC message vocabulary, no certification claim found |
| Access gate | `accredited-or-licensed` — GoStandard/GoGlobal IATA accreditation plus separate Jetstar approval |

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
