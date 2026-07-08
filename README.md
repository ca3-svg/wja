# WJA

WJA is a lightweight pairing PDF parser and bid-planning web app for airline pilots.
It turns monthly pairing documents into searchable, structured data so you can review trips, filter options, plan GDOs, and build a bid faster.

Current version: `v0.1.0`

## What It Does

- Upload a pairing PDF and extract the text locally in the browser.
- Parse trip blocks into structured fields like trip number, pairing number, base, dates, credit, TAFB, per diem, layovers, and legs.
- View the parsed pairings in a searchable, sortable table.
- Filter pairings by things like base, days, redeye, commutable, lazy, weekday-only, deadhead, and ETOPS-related flags.
- Plan guaranteed days off on a calendar view.
- Build and score a bid list with basic guardrails and export-friendly output.

## Why It Exists

Pairing PDFs are dense and hard to scan quickly.
WJA reduces the manual effort of reading monthly schedules by turning them into a cleaner workflow for:

- trip review
- pairing comparison
- bid selection
- schedule sanity checks

## Main Features

- PDF upload with client-side text extraction
- Final and prelim pairing parsing
- Searchable Tabulator-based pairing table
- Trip detail inspection
- GDO planner with calendar highlighting
- Bid builder with ranking and conflict checks
- Local persistence in browser storage
- Dark mode UI

## How It Works

1. Upload a pairing PDF.
2. The app uses `pdf.js` to read the text from each page.
3. The parser detects trip blocks and extracts useful fields.
4. Parsed trips are rendered into the table and calendar views.
5. You filter, compare, and assemble a bid list from the parsed data.

## Project Structure

- `index.htm` - main browser app
- `pairing_parser.py` - standalone Python parser that outputs JSON
- `CHANGELOG.md` - release history
- `RELEASE.md` - release/versioning notes
- `CONTRIBUTING.md` - contribution workflow
- `SECURITY.md` - security reporting guidance

## Usage

Open `index.htm` in a browser, upload a pairing PDF, and start filtering pairings.

## Tech Stack

- HTML5
- Vanilla JavaScript
- Tabulator
- PDF.js
- Tailwind CDN
- Python 3.11+ for the standalone parser

## Versioning

This repo uses semantic versioning.

- `MAJOR` for breaking changes
- `MINOR` for new features
- `PATCH` for fixes

## License

See [LICENSE](LICENSE).
