# R&D Log – Enrichora Project

## Introduction
Enrichora is a no‑scraping, API‑based lead‑enrichment SaaS for B2B agencies.  
Goal: Automate CSV lead enrichment (company, role, location, email hints) using APIs + AI, without scraping LinkedIn.

## Week 1 – Problem & Tech Research

- 2026-03-25:
  - Understood problem:
    - SaaS agencies manually enrich leads using LinkedIn, Google, Hunter, etc.
    - Need an automated system that:
      - Uploads CSVs.
      - Enriches data.
      - Tags source (e.g., "Hunter.io", "Company About page", "AI‑prediction").
      - Exports clean CSV.
  - Studied competitors:
    - Lusha, Apollo, Hunter, Clearbit, PDL, Gumloop, etc.
  - Decided approach:
    - No LinkedIn scraping.
    - Laravel + MySQL + n8n stack.
    - Hostinger cPanel hosting for MVP.
  - Created product‑requirement‑style PRD (`PRODUCT_REQUIREMENTS.md`).

## Week 2 – Setup LinkedIn Developer Access

- 2026-03-25:
  - Created LinkedIn Company Page: `Enrichora Labs`.
  - Went to LinkedIn Developer Portal: `https://developer.linkedin.com`.
  - Created developer app:
    - App name: `Enrichora Dev`.
    - Selected LinkedIn Company Page.
    - Added simple privacy‑policy URL (temporary GitHub Pages page).
    - Uploaded basic logo.
  - Successfully created app and saved:
    - `client_id` and `client_secret` safely in notes.
  - Researched LinkedIn API terms:
    - No scraping allowed.
    - Use only official APIs with proper consent and rate‑limits.
