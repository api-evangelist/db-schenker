# DB Schenker (db-schenker)

DB Schenker (Schenker AG, headquartered in Essen, Germany) is one of the world's largest freight forwarders and contract logistics providers, moving air, ocean, land and rail freight and running warehousing for shippers across roughly 1,850 locations. As a forwarder it sits in the intermediation layer of the supply chain — between the shipper who owns the cargo and the carriers, terminals and customs authorities who move and clear it — buying capacity it does not own and reselling visibility it did not have to publish. Its API posture is honestly a customer-contract posture, not a public developer posture. Deutsche Bahn sold DB Schenker to DSV A/S, completing 30 April 2025, and as of this profile www.dbschenker.com 301-redirects to dsv.com while the global developer portal at api-portal.dbschenker.com answers HTTP 410 Gone. The one DB Schenker-branded machine-readable API surface still live is the Nordic parcel "Partner services API" at parcelservices-se.dbschenker.com/Apipartner, which publishes four Swagger 2.0 documents openly but returns 401 on every operation without HTTP Basic credentials issued against a signed Swedish transport agreement. Its EDI endpoints are proprietary JSON, not EDIFACT or X12, and no DCSA, IATA ONE Record, GS1 EPCIS or WCO Data Model conformant contract was found on any reachable host.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/db-schenker/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/db-schenker/refs/heads/main/apis.yml)

## Tags

- Logistics
- Supply Chain
- Germany
- Freight Forwarding
- Parcel
- Track and Trace
- Customs
- Air Cargo
- Ocean Freight
- Contract Logistics
- EDI

## Timestamps

- **Created:** 2026-07-30
- **Modified:** 2026-07-30

## APIs

### DB Schenker Partner Services API V1

Version 1 of the Schenker AB (Sweden) Partner services API — the Nordic parcel network surface inherited from Privpak. Nine operations covering service point lookup (DeliveryPoint and ExtendedDeliveryPoint GetAllServicePoints / GetNearestServicePoint), shipment registration via POST /Edi/v1/RegisterEdi and /Edi/v1/RegisterReturnEdi, QR print codes, sorting-code resolution from sender/receiver postal codes and product code, and parcel track-and-trace by barcode. Swagger 2.0, HTTPS only, HTTP Basic authentication; every operation returned 401 unauthenticated when probed 2026-07-30.

- **Human URL:** [https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- **Base URL:** `https://parcelservices-se.dbschenker.com/Apipartner`

#### Tags

- Parcel
- Track and Trace
- EDI
- Service Points

#### Properties

- [OpenAPI](openapi/db-schenker-partner-services-v1-swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [API Reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [Documentation](https://parcelservices-se.dbschenker.com/Apipartner/Help)
- [Sandbox](https://staging-parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [SDK](https://parcelservices-se.dbschenker.com/Utils/PartnerServices/ParcelServicesExamples.zip)

### DB Schenker Partner Services API V2

Version 2 of the Schenker AB (Sweden) Partner services API. Four operations: DeliveryPoint/v2 GetServicePoint (by four-digit service point number), GetAllServicePoints and GetNearestServicePoint, plus TrackAndTraceAdvanced/v2/GetParcel which resolves a parcel and its event history from a country code, reference type and reference. Read-only polling; no webhook or subscription operation is published. Swagger 2.0, HTTP Basic authentication.

- **Human URL:** [https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- **Base URL:** `https://parcelservices-se.dbschenker.com/Apipartner`

#### Tags

- Parcel
- Track and Trace
- Service Points

#### Properties

- [OpenAPI](openapi/db-schenker-partner-services-v2-swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [API Reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [Documentation](https://www.dbschenker.com/resource/blob/488782/4dd6a5822abef794b803615c81a8725b/api-tracking-data.pdf)

### DB Schenker Partner Services API V3

Version 3 of the Schenker AB (Sweden) Partner services API, adding the parcel-box surface used in e-commerce checkout. Six operations across DeliveryPoint/v3: GetServicePoint, GetAllServicePoints, GetNearestServicePoint, GetBox, GetNearestBoxes and GetNearestTerminal. Backs the DB SCHENKERparcel box product; the published Parcelbox-API specification is version 1.3.0. Swagger 2.0, HTTP Basic authentication.

- **Human URL:** [https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- **Base URL:** `https://parcelservices-se.dbschenker.com/Apipartner`

#### Tags

- Parcel
- Parcel Box
- Service Points
- Checkout

#### Properties

- [OpenAPI](openapi/db-schenker-partner-services-v3-swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [API Reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [Documentation](https://www.dbschenker.com/resource/blob/837402/4a1ecfc7c167ca6fe2b1d676f41c9f2d/parcelbox-api-data.pdf)

### DB Schenker Partner Services API V4

Version 4 of the Schenker AB (Sweden) Partner services API, the current CollectionPoint surface (published specification version 4.2.0, document dated 2025-04-23). Six operations across DeliveryPoint/v4: GetServicePoint, GetAllServicePoints, GetNearestServicePoint, GetTerminal, GetAllTerminals and GetNearestTerminal — covering DB SCHENKERparcel ombud, ombud Europa, and DB SCHENKERparcel / DB SCHENKERsystem with the Collect at terminal option. DeliveryPoint v1 and v2 were withdrawn from support on 15 January 2025. Swagger 2.0, HTTP Basic authentication; a maximum 12-hour cache is mandated on collection point data.

- **Human URL:** [https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- **Base URL:** `https://parcelservices-se.dbschenker.com/Apipartner`

#### Tags

- Parcel
- Service Points
- Terminals
- Checkout

#### Properties

- [OpenAPI](openapi/db-schenker-partner-services-v4-swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [API Reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [Documentation](https://www.dbschenker.com/resource/blob/488786/f0364447f37034a10f72e0768fc110ef/collectionpointinfo-data.pdf)

## Common Properties

- [Website](https://www.dbschenker.com/)
- [API Reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [Documentation](https://parcelservices-se.dbschenker.com/Apipartner/Help)
- [GitHub Organization](https://github.com/dbschenker)
- [LinkedIn](https://www.linkedin.com/company/db-schenker)
- [Support Documentation](https://help.eschenker.dbschenker.com/helpsystem/content/)
- [Successor Organization](https://www.dsv.com/en)

## Interoperability

A shipment crosses many parties. What matters is whether what DB Schenker publishes can be spoken by the next party in the chain. See [review.yml](review.yml) for the full evidence trail and every probed URL with its HTTP status.

| Dimension | Finding |
| --- | --- |
| Standard conformance | No standard reference found — no DCSA, IATA ONE Record, Cargo-XML, GS1 EPCIS, UN/CEFACT MMT, WCO Data Model, eFTI or MLETR reference on any reachable host |
| Interface shape | `proprietary-documented` — versioned, machine-readable, publicly fetchable, and shared with nobody |
| Identifier scheme | Carrier-private shipment number, colli ID / barcode, four-digit service point number, terminal code, Box ID, plus ISO country and postal codes. No GS1, container, B/L, AWB, UN/LOCODE, SCAC or EORI identifiers |
| Event model | `polling-only` — GetParcel returns an Events array; no webhook, subscription or AsyncAPI operation exists, and the docs mandate 12-hour re-polling |
| EDI legacy | `RegisterEdi` / `RegisterReturnEdi` are proprietary JSON, not EDIFACT or X12; eSchenker used XML file drop plus an administrator-issued Access Key; no VAN or AS2 referenced |
| Multi-party posture | Publishes downward to contracted shippers and their TA/ERP or checkout integrators only; nothing a carrier or peer forwarder could consume back |
| Access gate | `customer-account-required` — a country transport agreement, an authorization request, then HTTP Basic credentials |
| Ocean / DCSA | Not a DCSA member (forwarder, not a vessel operator) and publishes no DCSA-conformant contract; there is no ocean-freight API under dbschenker.com at all |

## Corporate status

Deutsche Bahn completed the sale of DB Schenker to **DSV A/S** on **30 April 2025**. As of 2026-07-30 the estate is visibly mid-migration:

- `www.dbschenker.com`, `schenker.com`, `connect.dbschenker.com`, `www.schenker.se`, `www.dbschenker.se` and `www.dbschenker.fi` all **301 to dsv.com**
- `api-portal.dbschenker.com` — the former global developer portal — answers **HTTP 410 Gone**
- `help.eschenker.dbschenker.com` still serves, now branded **myDSV Online Help**
- `developer.logisticstechnology.no` still titles itself "DB Schenker APIs" but its footer reads **"2026 © DSV Road AS"**; its APIs are attributed to DSV, not to DB Schenker, in this profile
- `parcelservices-se.dbschenker.com/Apipartner` remains live and DB Schenker-branded, and is the source of all four harvested specifications
