# Mileage Tracker v4

Single-user web application for IRS substantiation-grade mileage logging with receipt capture.

## Features

- Authentication (Argon2id, session-based)
- Vehicle management with per-tax-year odometer readings
- Trip CRUD with IRC §274(d) substantiation fields
- Time-effective IRS mileage rates (DB reference data)
- Deduction calculation and year-end summary
- CSV and PDF export
- Polished UI with design tokens, dark mode, and mobile-responsive layout
- **Receipt capture**: upload multiple images per trip (JPEG/PNG/WebP/HEIC), ownership-gated display, export references

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python run.py
```

Open http://127.0.0.1:8000 — register the first user, then log trips and attach receipts.

## Branch

Implementation target: `feat/mvp-v4` on `raghu-cmyk/mileage-tracker-v4`.
