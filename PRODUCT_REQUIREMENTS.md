# Enrichora – Product Requirements (v1)

## Vision
Enrichora is a **no‑scraping, API‑based lead‑enrichment SaaS** that helps SaaS agencies and sales teams upload messy CSVs of leads and get **enriched, deduplicated, source‑tagged contacts** without scraping LinkedIn.

## Key Features
- CSV upload → enrichment → export.
- Source‑tagged data (e.g., "Hunter.io", "Company About page", "AI‑prediction").
- Credit‑based usage (1 credit per lead / search, 3 per CSV export).
- Simple UI: Laravel + Blade.

## Tech Stack
- Backend: Laravel 10/11.
- DB: MySQL.
- Hosting: Hostinger cPanel (`skailabz.com` / subdomain).
- Automation: n8n for API workflows.
- Data sources:
  - Hunter / email‑finder APIs.
  - Clearbit / PDL / domain‑enrichment APIs.
  - LinkedIn API (official, no scraping, only for login / small‑scope enrichment).

## Out of Scope (MVP)
- LinkedIn scraping (Chrome extension, headless‑browser).
- Real‑time streaming / live‑sync.
- Complex AI models (beyond simple prediction for role / industry / seniority).
