<div align="center">

<img src="brand/logo.svg" alt="MEDNEXA" width="200" />

# MEDNEXA

**Connecting Healthcare.**

Egyptian mid-market healthcare integration platform — HIS × LIS × PACS wiring with HL7v2, FHIR R4, DICOM, and PDPC-compliant audit built in from day one.

**Status: Pilot-ready · Session 01 complete · 128/128 engine tests green**

</div>

---

> This repository is a **public showcase**. The strategy, financial model, pilot sales package, and signed-DPA templates are retained as commercial artifacts. The engine source itself remains under commercial license — reach out for an evaluation copy.
>
> Everything on this page is externally verifiable.

---

## What MEDNEXA actually ships

- **FastAPI engine** (Python 3.12) · 80+ REST routes exposing FHIR R4 resources, HL7v2 ingestion, DICOM metadata, and audit queries
- **Real DIMSE SCP** · receives `C-STORE` and `C-FIND Modality Worklist` on port `11112`
- **HL7v2 message parser** · `ADT` / `ORM` / `ORU` / `OUL` / `MDM` hand-off into FHIR builders
- **FHIR R4 builders** · `Observation`, `DiagnosticReport`, `ServiceRequest`, `Patient`, `Practitioner`
- **DICOM in-browser viewer** · Cornerstone.js on `/app/dicom-viewer.html` for sample CT studies
- **Report state-machine** · `draft → signed → finalized → amended` with audit trace at every transition
- **Hash-chained audit log** · SHA-256 `prev_hash + hash` per entry so any mutation after the fact is detectable
- **MFA TOTP** (RFC 6238) · AES-256-GCM encrypted secrets at rest
- **Refresh-token rotation** · SHA-256-hashed tokens, old token invalidated on first use of its successor
- **Sliding-window rate limits** · per-IP and per-user
- **Bilingual UI** · Arabic RTL + English LTR, Clinical Editorial design system (Sage / Cream / editorial-serif)
- **nginx 1.27 reverse proxy** · CSP, HSTS, X-Frame-Options wired on the public TLS endpoint
- **128 automated engine tests** · 100% passing on the pre-pilot build

## Compliance posture

- **PDPC (Egypt Law 151/2020)** · consent management, data-subject rights, retention policies, cross-border transfer gating
- **HIPAA alignment** · encrypted PHI at rest + in transit, access logs, break-glass with mandatory audit
- **DPA + SLA templates** · available on request for pilot evaluations

## Design system

A dedicated "Clinical Editorial" system — calm sage greens on cream, editorial serif pairings, zero bright reds except for critical patient-safety alerts. The design philosophy prefers trust and legibility over SaaS exuberance.

Brand materials in [`brand/`](brand/) — `logo.svg`, `logo-icon.svg`, and [`brand/BRAND_GUIDE.md`](brand/BRAND_GUIDE.md).

## Four demo accounts (on pilot deployments)

| Role | Description |
|---|---|
| Admin | Full administrative view, audit trail, patient roster |
| Radiologist | Report authoring, DICOM viewer, state-machine transitions |
| Doctor (referring) | Scoped-ACL view — sees only patients explicitly consented to them, per admin approval |
| Patient | Owns study / report access, grants or revokes consent per practitioner |

Pilot deployments publish these on a Cloudflare-tunnelled TLS host. Request access via `abdarahman10555@gmail.com`.

## Related projects in the Nexus Zone ecosystem

- **midcine** · Arabic Cloud-Native RIS/PACS — 24-slice CT → structured Arabic DICOM SR in ~69 s · [github.com/61465/midcine](https://github.com/61465/midcine)
- **NEXUS-AI** · 134-agent MCP orchestration framework used in MEDNEXA's inference pipeline · [github.com/61465/NEXUS-AI](https://github.com/61465/NEXUS-AI)
- **Nexus Zone portfolio companion** · [61465.github.io/Nexus_Zone_Portfolio_Companion](https://61465.github.io/Nexus_Zone_Portfolio_Companion/)

## What is NOT in this repository

The following live under commercial license and are shared under NDA for pilot discussions:

- `strategy/` — market validation, competitive analysis, Egyptian mid-market go-to-market
- `deck/` — 15-slide pitch, 36-month × 3-scenario financial model
- `sales/` — discovery questionnaire (30 Qs), proposal template, SOW, DPA (PDPC Law 151/2020 aligned), demo script, ROI calculator, pilot case-study framework
- `engine/` source — FastAPI code, DICOM SCP, HL7v2 parser, FHIR builders, auth stack, audit chain
- Hospital-side integration playbooks

## Contact

**Abd Alrahaman Mohamed** · founder & lead engineer
`abdarahman10555@gmail.com` · [github.com/61465](https://github.com/61465)

For pilot evaluations, DPA requests, or technical due diligence, email with "MEDNEXA pilot" in the subject.

---

<div align="center">

**Nexus Zone** · Building serious healthcare software for the Arab world.

</div>
