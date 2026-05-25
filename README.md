# CAMARA Project (camara-project)
CAMARA is the Telco Global API Alliance — an open-source project hosted by the Linux Foundation that defines, builds, and tests a unified set of network APIs across the world's mobile operators. Working alongside the GSMA Open Gateway commercialization initiative, CAMARA produces operator-neutral OpenAPI 3.0 specifications for 60+ telco network capabilities including Number Verification, SIM Swap, Device Location, Quality on Demand, KYC, Carrier Billing, Edge Discovery, Device Status, SMS, and more — all published under Apache 2.0.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/apis.yml)

**Type:** `standard` (open-source spec project under the Linux Foundation)

## Tags

API Standards, CAMARA, GSMA, Linux Foundation, Network APIs, Open API, Open Gateway, Open Source, Standards, Telco, Telco API Alliance, Telecom, Telecommunications

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Governance and Structure

CAMARA is governed by:

- **Technical Steering Committee** — oversight body for the technical CAMARA Project
- **Governing Board** — manages the Directed Fund (budget, outreach, officer elections)
- **End User Council** — composed of API end users
- **Working Groups and Sub-Projects** — each API or cross-cutting concern lives in its own repo

Repositories progress through three maturity levels:

1. **Sandbox** — initial proposal, exploratory work
2. **Incubating** — actively developed, draft OpenAPI in place
3. **Graduated** — stable, released, multi-operator implementations

Cross-cutting working groups define shared rules:

- **[Commonalities](https://github.com/camaraproject/Commonalities)** — API design guide, error model, shared data types
- **[Identity And Consent Management](https://github.com/camaraproject/IdentityAndConsentManagement)** — OIDC CIBA flow, purpose-bound consent scopes
- **[Release Management](https://github.com/camaraproject/ReleaseManagement)** — coordinated quarterly Meta-Releases (e.g. Spring25, Fall25)
- **[APIBacklog](https://github.com/camaraproject/APIBacklog)** — central pipeline of proposed APIs

## Profiled APIs

This catalog profiles 15 of the most-mature CAMARA APIs in detail. The full CAMARA portfolio covers 60+ APIs; see the [GitHub organization](https://github.com/camaraproject) for the complete list.

### CAMARA Number Verification API
Verify or retrieve the mobile phone number currently allocated by the network to the SIM in the user's device, using silent network/SIM-based authentication (no SMS OTP). Used at sign-up, login, or transaction time.

- [Repository](https://github.com/camaraproject/NumberVerification)
- [OpenAPI](openapi/number-verification-openapi.yml)

### CAMARA SIM Swap API
Detect whether the SIM behind a phone number was recently swapped — a key anti-fraud signal for banking, fintech, and any SMS-OTP-based flow. Includes an on-demand query endpoint and a CloudEvents subscription endpoint.

- [Repository](https://github.com/camaraproject/SimSwap)
- [OpenAPI — sim-swap](openapi/sim-swap-openapi.yml)
- [OpenAPI — sim-swap-subscriptions](openapi/sim-swap-subscriptions-openapi.yml)

### CAMARA Device Location API
Network-derived device location (not GPS), location verification against a target area, and geofencing event subscriptions.

- [Repository](https://github.com/camaraproject/DeviceLocation)
- [OpenAPI — Location Retrieval](openapi/device-location-retrieval-openapi.yml)
- [OpenAPI — Location Verification](openapi/device-location-verification-openapi.yml)
- [OpenAPI — Geofencing Subscriptions](openapi/device-location-geofencing-openapi.yml)

### CAMARA Quality on Demand API
Request boosted QoS (committed bandwidth, low latency, priority) for a specific device-application session — the foundational 5G monetization API.

- [Repository](https://github.com/camaraproject/QualityOnDemand)
- [OpenAPI — Quality on Demand](openapi/quality-on-demand-openapi.yml)
- [OpenAPI — QoS Profiles](openapi/qos-profiles-openapi.yml)
- [OpenAPI — QoS Provisioning](openapi/qos-provisioning-openapi.yml)

### CAMARA Device Status API
Device reachability, roaming state, and connected network type (2G/3G/4G/5G/NB-IoT).

- [Repository](https://github.com/camaraproject/DeviceStatus)
- [OpenAPI — Connected Network Type](openapi/device-status-connected-network-type-openapi.yml)
- [OpenAPI — Reachability](openapi/device-status-reachability-openapi.yml)
- [OpenAPI — Roaming](openapi/device-status-roaming-openapi.yml)

### CAMARA Know Your Customer API
Three KYC surfaces — KYC Match (score supplied attributes against operator records), KYC Fill-In (operator pre-populates onboarding fields), KYC Age Verification (over-N check without revealing DOB).

- [Repository](https://github.com/camaraproject/KnowYourCustomer)
- [OpenAPI — KYC Match](openapi/kyc-match-openapi.yml)
- [OpenAPI — KYC Fill-In](openapi/kyc-fill-in-openapi.yml)
- [OpenAPI — KYC Age Verification](openapi/kyc-age-verification-openapi.yml)

### CAMARA One Time Password SMS API
Operator-delivered OTP send + validate. Higher deliverability and trust than third-party SMS aggregators.

- [Repository](https://github.com/camaraproject/OTPValidation)
- [OpenAPI](openapi/one-time-password-sms-openapi.yml)

### CAMARA Device Swap API
Detect whether the device (IMEI) behind a phone number has recently changed. Complements SIM Swap as an account-takeover signal.

- [Repository](https://github.com/camaraproject/DeviceSwap)
- [OpenAPI](openapi/device-swap-openapi.yml)

### CAMARA Simple Edge Discovery API
Discover the optimal Multi-access Edge Computing (MEC) endpoint for a given device based on its current network attachment.

- [Repository](https://github.com/camaraproject/SimpleEdgeDiscovery)
- [OpenAPI](openapi/simple-edge-discovery-openapi.yml)

### CAMARA Carrier Billing Checkout API
Direct Carrier Billing — charge against the subscriber's mobile bill, with refund support.

- [Repository](https://github.com/camaraproject/CarrierBillingCheckOut)
- [OpenAPI](openapi/carrier-billing-openapi.yml)

### CAMARA Population Density Data API
Aggregated, anonymized device counts in a geographic area over a time window. Smart-city, retail, event, and emergency-response use cases.

- [Repository](https://github.com/camaraproject/PopulationDensityData)
- [OpenAPI](openapi/population-density-data-openapi.yml)

### CAMARA Home Devices Quality on Demand API
Quality on Demand for fixed-broadband home networks — boost a device behind a home gateway for a bounded window.

- [Repository](https://github.com/camaraproject/HomeDevicesQoD)
- [OpenAPI](openapi/home-devices-qod-openapi.yml)

### CAMARA Call Forwarding Signal API
Detect whether a subscriber currently has call forwarding configured (unconditional, busy, no-reply, unreachable). Anti-fraud signal for voice OTP flows.

- [Repository](https://github.com/camaraproject/CallForwardingSignal)
- [OpenAPI](openapi/call-forwarding-signal-openapi.yml)

### CAMARA Short Message Service API
Programmatic SMS send with CloudEvents delivery-status callbacks.

- [Repository](https://github.com/camaraproject/ShortMessageService)
- [OpenAPI](openapi/sms-openapi.yml)

### CAMARA Connectivity Insights API
Real-time throughput, latency, jitter, and signal-quality insights for adaptive applications.

- [Repository](https://github.com/camaraproject/ConnectivityInsights)
- [OpenAPI](openapi/connectivity-insights-openapi.yml)

## Additional CAMARA APIs

CAMARA's full portfolio also includes (sample): Edge Cloud, Optimal Edge Discovery, Application Endpoint Discovery / Registration, Edge Application Management, Device Identifier, Device Authenticity, eSIM Remote Management, IoT Device Management, IoT SIM Fraud Prevention, IoT Network Optimization, Network Slice Booking, Dedicated Networks, Multi-Point VPN, Site-to-Cloud VPN, Region Device Count, Most Frequent Location, Device Visit Location, Predictive Connectivity Data, Network Insights, Customer Insights, Session Insights, Subscription Status, Verified Caller, Number Recycling, Tenure, Click to Dial, WebRTC, Voice Notification, Voice Verification Code, Sponsored Data, Consent Info / Consent Management, Blockchain Public Address, Energy Footprint Notification, Traffic Influence, QoS Booking, Model as a Service, Rainfall Intensity, Connected Network Type, Device Reachability Status, Device Roaming Status, Capabilities and Runtime Restrictions, In-Home Device Management, High-Throughput Elastic Networks, and more. Each lives in its own repo at [github.com/camaraproject](https://github.com/camaraproject).

## Common Properties

- [Portal — camaraproject.org](https://camaraproject.org)
- [About — CAMARA](https://camaraproject.org/about-camara/)
- [GitHub Organization](https://github.com/camaraproject)
- [Governance](https://github.com/camaraproject/Governance)
- [Project Charter](https://github.com/camaraproject/Governance/blob/main/ProjectCharter.md)
- [Commonalities (API Design Guidelines)](https://github.com/camaraproject/Commonalities)
- [Identity And Consent Management](https://github.com/camaraproject/IdentityAndConsentManagement)
- [Release Management](https://github.com/camaraproject/ReleaseManagement)
- [API Backlog](https://github.com/camaraproject/APIBacklog)
- [Wiki](https://wiki.camaraproject.org/)
- [Swagger UI for all APIs](https://camaraproject.github.io/)
- [Code of Conduct](https://github.com/camaraproject/Governance/blob/main/CODE_OF_CONDUCT.md)
- [Contributing](https://github.com/camaraproject/Governance/blob/main/CONTRIBUTING.md)
- [License (Apache 2.0)](https://github.com/camaraproject/Governance/blob/main/documentation/LICENSE.APACHE2.0)
- [Mailing Lists](https://lists.camaraproject.org/g/all)
- [News and Events](https://camaraproject.org/news-and-events/)
- [Linux Foundation Announcement](https://www.linuxfoundation.org/press/announcing-camara-the-telco-global-api-alliance)
- [GSMA Open Gateway (commercialization partner)](https://www.gsma.com/solutions-and-impact/connectivity-for-good/external-affairs/wp-content/uploads/2024/02/Open-Gateway-Joint-Statement.pdf)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Number Verification](openapi/number-verification-openapi.yml)
- [SIM Swap](openapi/sim-swap-openapi.yml)
- [SIM Swap Subscriptions](openapi/sim-swap-subscriptions-openapi.yml)
- [Device Location — Retrieval](openapi/device-location-retrieval-openapi.yml)
- [Device Location — Verification](openapi/device-location-verification-openapi.yml)
- [Device Location — Geofencing Subscriptions](openapi/device-location-geofencing-openapi.yml)
- [Quality on Demand](openapi/quality-on-demand-openapi.yml)
- [QoS Profiles](openapi/qos-profiles-openapi.yml)
- [QoS Provisioning](openapi/qos-provisioning-openapi.yml)
- [Device Status — Connected Network Type](openapi/device-status-connected-network-type-openapi.yml)
- [Device Status — Reachability](openapi/device-status-reachability-openapi.yml)
- [Device Status — Roaming](openapi/device-status-roaming-openapi.yml)
- [KYC — Match](openapi/kyc-match-openapi.yml)
- [KYC — Fill-In](openapi/kyc-fill-in-openapi.yml)
- [KYC — Age Verification](openapi/kyc-age-verification-openapi.yml)
- [One Time Password SMS](openapi/one-time-password-sms-openapi.yml)
- [Device Swap](openapi/device-swap-openapi.yml)
- [Simple Edge Discovery](openapi/simple-edge-discovery-openapi.yml)
- [Carrier Billing](openapi/carrier-billing-openapi.yml)
- [Population Density Data](openapi/population-density-data-openapi.yml)
- [Home Devices QoD](openapi/home-devices-qod-openapi.yml)
- [Call Forwarding Signal](openapi/call-forwarding-signal-openapi.yml)
- [SMS](openapi/sms-openapi.yml)
- [Connectivity Insights](openapi/connectivity-insights-openapi.yml)

All specifications are mirrored verbatim from each working group's canonical `code/API_definitions/*.yaml` at the time of capture.

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
