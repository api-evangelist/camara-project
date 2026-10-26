# CAMARA Project (camara-project)

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

CAMARA is the Telco Global API Alliance — an open-source project hosted by the Linux Foundation that defines, builds, and tests a unified set of network APIs across the world's mobile operators. Working alongside the GSMA Open Gateway commercialization initiative, CAMARA produces operator-neutral OpenAPI 3.0 specifications for 60+ telco network capabilities including Number Verification, SIM Swap, Device Location, Quality on Demand, KYC, Carrier Billing, Edge Discovery, Device Status, SMS, and more — all published under Apache 2.0. The project is organized into Sandbox, Incubating, and Graduated sub-projects with cross-cutting Commonalities, Identity and Consent Management, and Release Management working groups. Major contributors include Deutsche Telekom, Orange, Telefonica, Vodafone, T-Mobile, Verizon, AT&T, KDDI, SK Telecom, China Mobile, and dozens of other operators and vendors.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- API Standards
- CAMARA
- GSMA
- Linux Foundation
- Network APIs
- Open API
- Open Gateway
- Open Source
- Standards
- Telco
- Telco API Alliance
- Telecom
- Telecommunications

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### CAMARA Number Verification API

Verify or retrieve the mobile phone number currently allocated by the network operator to the SIM in the end user's device. Uses silent network-based or SIM-based authentication (no SMS OTP, no app download) to confirm possession of a phone number at sign-up, login, or transaction time. Returns true/false on verify or the masked phone number on retrieve.

- **Human URL:** [https://github.com/camaraproject/NumberVerification](https://github.com/camaraproject/NumberVerification)

#### Tags

- Authentication
- Identity
- Number Verification
- Phone Number
- Silent Auth
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/NumberVerification)
- [OpenAPI](openapi/number-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/number-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/number-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA SIM Swap API

Detect whether the SIM associated with a mobile phone number has recently been swapped to a different SIM. Returns the most recent SIM swap timestamp or a boolean check for a configurable look-back period. Critical fraud signal for banking, fintech, crypto, and any service relying on SMS OTP. Includes both an on-demand query API and an event subscriptions API for CloudEvents push notifications.

- **Human URL:** [https://github.com/camaraproject/SimSwap](https://github.com/camaraproject/SimSwap)

#### Tags

- Anti-Fraud
- Fraud Prevention
- Identity
- SIM Swap
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/SimSwap)
- [OpenAPI](openapi/sim-swap-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sim-swap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sim-swap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/sim-swap-subscriptions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sim-swap-subscriptions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sim-swap-subscriptions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Device Location API

Retrieve the network-derived location of a mobile device, verify whether a device is within a given geographic area, or subscribe to geofencing entry/exit events. Location is provided by the mobile operator based on the network's view of the device — not from device GPS — so it works without an app, cannot be spoofed by GPS, and can be used for fraud detection, regulatory verification, and asset tracking.

- **Human URL:** [https://github.com/camaraproject/DeviceLocation](https://github.com/camaraproject/DeviceLocation)

#### Tags

- Device Location
- Geofencing
- Location
- Location Verification
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/DeviceLocation)
- [OpenAPI](openapi/device-location-retrieval-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-location-retrieval.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-location-retrieval.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/device-location-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-location-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-location-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/device-location-geofencing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-location-geofencing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-location-geofencing.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Quality on Demand API

Request elevated network Quality of Service for a specific device-application session — committed bandwidth, low latency, or prioritized traffic — for a bounded time window. Includes a profiles catalog (discover available QoS classes), session management (create/get/delete QoS sessions), and a provisioning surface for longer-lived attachments. Foundational 5G monetization API.

- **Human URL:** [https://github.com/camaraproject/QualityOnDemand](https://github.com/camaraproject/QualityOnDemand)

#### Tags

- 5G
- Network Slicing
- QoS
- Quality on Demand
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/QualityOnDemand)
- [OpenAPI](openapi/quality-on-demand-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/quality-on-demand.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/quality-on-demand.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/qos-profiles-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qos-profiles.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qos-profiles.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/qos-provisioning-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qos-provisioning.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qos-provisioning.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Device Status API

Query whether a mobile device is reachable on the network, currently roaming, and what type of network it is connected to (2G, 3G, 4G, 5G, NB-IoT). Used by IoT fleet management, customer support diagnostics, and pre-flight checks before invoking other CAMARA APIs.

- **Human URL:** [https://github.com/camaraproject/DeviceStatus](https://github.com/camaraproject/DeviceStatus)

#### Tags

- Connected Network Type
- Device Status
- Reachability
- Roaming
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/DeviceStatus)
- [OpenAPI](openapi/device-status-connected-network-type-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-status-connected-network-type.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-status-connected-network-type.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/device-status-reachability-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-status-reachability.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-status-reachability.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/device-status-roaming-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-status-roaming.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-status-roaming.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Know Your Customer API

KYC sub-project bundling three identity APIs. KYC Match scores a supplied set of customer attributes (name, address, DOB, document number, etc.) against the operator's records. KYC Fill-In returns operator-held customer attributes to pre-populate an onboarding form. KYC Age Verification returns whether the subscriber is over a minimum age threshold without disclosing the date of birth.

- **Human URL:** [https://github.com/camaraproject/KnowYourCustomer](https://github.com/camaraproject/KnowYourCustomer)

#### Tags

- Age Verification
- Identity
- Identity Verification
- KYC
- Know Your Customer
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/KnowYourCustomer)
- [OpenAPI](openapi/kyc-match-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kyc-match.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kyc-match.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/kyc-fill-in-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kyc-fill-in.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kyc-fill-in.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/kyc-age-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kyc-age-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kyc-age-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA One Time Password SMS API

Send a one-time password via SMS to a target phone number and validate the code returned by the user. Operator delivers the SMS through the home network, so messages bypass third-party aggregators and inherit higher deliverability and trust.

- **Human URL:** [https://github.com/camaraproject/OTPValidation](https://github.com/camaraproject/OTPValidation)

#### Tags

- Authentication
- OTP
- One Time Password
- SMS
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/OTPValidation)
- [OpenAPI](openapi/one-time-password-sms-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/one-time-password-sms.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/one-time-password-sms.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Device Swap API

Detect whether the device (IMEI) associated with a phone number has recently changed. Complements SIM Swap as a fraud signal — a fresh device or SIM behind a known phone number can indicate account takeover.

- **Human URL:** [https://github.com/camaraproject/DeviceSwap](https://github.com/camaraproject/DeviceSwap)

#### Tags

- Anti-Fraud
- Device
- Device Swap
- Fraud Prevention
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/DeviceSwap)
- [OpenAPI](openapi/device-swap-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/device-swap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/device-swap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Simple Edge Discovery API

Discover the optimal Multi-access Edge Computing (MEC) endpoint for a given client device. The operator returns the closest edge data center URL based on the device's current network attachment so latency-sensitive applications (gaming, AR/VR, real-time inference) can route to the nearest compute.

- **Human URL:** [https://github.com/camaraproject/SimpleEdgeDiscovery](https://github.com/camaraproject/SimpleEdgeDiscovery)

#### Tags

- Edge Cloud
- Edge Computing
- MEC
- Simple Edge Discovery
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/SimpleEdgeDiscovery)
- [OpenAPI](openapi/simple-edge-discovery-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simple-edge-discovery.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simple-edge-discovery.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Carrier Billing Checkout API

Direct Carrier Billing checkout — initiate a one-time or recurring charge against the subscriber's mobile phone bill, with confirmation and refund flows. Lets merchants accept payment from users without a card or bank account.

- **Human URL:** [https://github.com/camaraproject/CarrierBillingCheckOut](https://github.com/camaraproject/CarrierBillingCheckOut)

#### Tags

- Billing
- Carrier Billing
- Direct Carrier Billing
- Payments
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/CarrierBillingCheckOut)
- [OpenAPI](openapi/carrier-billing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/carrier-billing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/carrier-billing.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Population Density Data API

Aggregated, anonymized counts of mobile devices observed in a target geographic area over a time window. Powers smart-city planning, retail footfall analytics, event crowd management, and emergency response — without exposing any individual identifier.

- **Human URL:** [https://github.com/camaraproject/PopulationDensityData](https://github.com/camaraproject/PopulationDensityData)

#### Tags

- Analytics
- Network Insights
- Population Density
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/PopulationDensityData)
- [OpenAPI](openapi/population-density-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/population-density-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/population-density-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Home Devices Quality on Demand API

Quality on Demand applied to fixed-broadband home networks — request boosted bandwidth or prioritized traffic for a specific device behind a home gateway for a bounded time window.

- **Human URL:** [https://github.com/camaraproject/HomeDevicesQoD](https://github.com/camaraproject/HomeDevicesQoD)

#### Tags

- Broadband
- Home Network
- QoS
- Quality on Demand
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/HomeDevicesQoD)
- [OpenAPI](openapi/home-devices-qod-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/home-devices-qod.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/home-devices-qod.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Call Forwarding Signal API

Detect whether a subscriber currently has unconditional, busy, no-reply, or unreachable call forwarding configured. Fraud signal used in conjunction with SIM Swap and Number Verification to detect account-takeover attempts that re-route voice OTPs.

- **Human URL:** [https://github.com/camaraproject/CallForwardingSignal](https://github.com/camaraproject/CallForwardingSignal)

#### Tags

- Anti-Fraud
- Call Forwarding
- Fraud Prevention
- Telecom
- Voice

#### Properties

- [Documentation](https://github.com/camaraproject/CallForwardingSignal)
- [OpenAPI](openapi/call-forwarding-signal-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/call-forwarding-signal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/call-forwarding-signal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Short Message Service API

Send SMS messages programmatically with operator-delivered routing. Includes a delivery-notification subscription surface for CloudEvents callbacks on message status (delivered, failed, expired).

- **Human URL:** [https://github.com/camaraproject/ShortMessageService](https://github.com/camaraproject/ShortMessageService)

#### Tags

- Messaging
- SMS
- Short Message Service
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/ShortMessageService)
- [OpenAPI](openapi/sms-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sms.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sms.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CAMARA Connectivity Insights API

Real-time connectivity quality insights — measured throughput, latency, jitter, and signal classification — for a target device. Used by applications to adapt quality (bitrate, codec, fallback) to real network conditions, or to trigger a Quality on Demand session when needed.

- **Human URL:** [https://github.com/camaraproject/ConnectivityInsights](https://github.com/camaraproject/ConnectivityInsights)

#### Tags

- Analytics
- Connectivity
- Insights
- Telecom

#### Properties

- [Documentation](https://github.com/camaraproject/ConnectivityInsights)
- [OpenAPI](openapi/connectivity-insights-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/connectivity-insights.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/connectivity-insights.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://camaraproject.org)
- [About Us](https://camaraproject.org/about-camara/)
- [GitHub Organization](https://github.com/camaraproject)
- [Documentation](https://github.com/camaraproject/Governance)
- [Documentation](https://github.com/camaraproject/Governance/blob/main/ProjectCharter.md)
- [Documentation](https://github.com/camaraproject/Commonalities)
- [Documentation](https://github.com/camaraproject/IdentityAndConsentManagement)
- [Documentation](https://github.com/camaraproject/ReleaseManagement)
- [Documentation](https://github.com/camaraproject/APIBacklog)
- [Documentation](https://wiki.camaraproject.org/)
- [Documentation](https://camaraproject.github.io/)
- [Contact](https://camaraproject.org/contact/)
- [Code Of Conduct](https://github.com/camaraproject/Governance/blob/main/CODE_OF_CONDUCT.md)
- [Documentation](https://github.com/camaraproject/Governance/blob/main/CONTRIBUTING.md)
- [License](https://github.com/camaraproject/Governance/blob/main/documentation/LICENSE.APACHE2.0)
- [Forum](https://lists.camaraproject.org/g/all)
- [Blog](https://camaraproject.org/news-and-events/)
- [Events](https://camaraproject.org/events/)
- [Press Release](https://www.linuxfoundation.org/press/announcing-camara-the-telco-global-api-alliance)
- [Partner](https://www.gsma.com/solutions-and-impact/connectivity-for-good/external-affairs/wp-content/uploads/2024/02/Open-Gateway-Joint-Statement.pdf)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
