# Clinic (Telemedicine) — Manual Testing Case Study

**SUT (System Under Test):**(https://github.com/Mdtanzidhossain/Online_clinic-website-_-CLINICARE_with-php-php-project-3.git)  
**Scope:** Manual testing only. No app code copied here.

## Goal
Validate end-to-end patient flows: registration/OTP, profile, doctor search/filter, slot booking/reschedule/cancel, report access, and notifications—ensuring correctness, robustness, and data integrity.

## What’s Included
- TEST_PLAN.md
- FEATURE_LIST.md
- CHECKLIST.md
- TEST_CASES.csv (starter set; expand as needed)
- RTM.md (requirements ↔ test cases)
- RESULTS.md (execution logs)
- BUG_REPORT_TEMPLATE.md

## STLC Followed (Concise)
Requirements review → Test planning → Test design (cases/charters) → Environment/data prep → Test execution → Defect reporting → Re-test & regression → Closure report.

## Assumptions
- OTP service returns a test code in non-prod.
- Email/SMS gateways are stubbed or observable via logs.
- Timezone defaults to Asia/Dhaka.

## How to Use This Repo
1) Read `TEST_PLAN.md` and `FEATURE_LIST.md`.  
2) Execute cases in `TEST_CASES.csv`.  
3) Record outcomes in `RESULTS.md` and open issues using `BUG_REPORT_TEMPLATE.md`.  
4) Keep `RTM.md` updated when adding cases.

> Anonymized, documentation-only portfolio. Full artifacts available under NDA on request.
