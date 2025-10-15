# Test Plan — Clinic (Telemedicine)

## 1. Objectives
- Validate core patient journeys: account, doctor discovery, appointment lifecycle, records access.
- Prove reliability on boundary inputs (dates, timezones, conflicts).
- Ensure privacy controls on PII.

## 2. In Scope
- Web app patient-facing flows (if applicable) / mobile web.
- OTP, profile, booking, cancel/reschedule, notifications, records view/download.

## 3. Out of Scope
- Provider onboarding flows, payments gateway certification, video-call SDK internals.

## 4. Test Types
Functional (Pos/Neg/Edge), Usability (heuristic), Accessibility (quick checks), Data validation, Localization (date/time), Non-functional smoke (basic performance hints).

## 5. Environments
- Staging/local build of SUT repo
- TZ: Asia/Dhaka

## 6. Test Data Strategy
- Synthetic users (PAT_###). Doctors (DOC_###). Slots as YYYY-MM-DD HH:mm, include overlaps and invalid ranges.

## 7. Entry/Exit Criteria
Entry: SUT deployable; stable endpoints; test users available.  
Exit: ≥95% high-priority cases pass; no open Sev-1/Sev-2; key risks mitigated.

## 8. Risks & Mitigations
- OTP flakiness → capture logs & fallback test OTP.
- Timezone drift → assert UTC+6 conversions.
- PII exposure → verify masked views and secured downloads.

## 9. KPIs
Pass rate, defect density, retest cycle time, escaped defects (0 target).

> Anonymized, documentation-only portfolio. Full artifacts available under NDA on request.
