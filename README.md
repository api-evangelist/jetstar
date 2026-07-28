# Jetstar (jetstar)

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
