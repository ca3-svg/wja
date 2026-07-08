# ✈️ Pairing Parser Web App

A lightweight, self-hosted PDF pairing schedule parser and viewer built for airline pilots.  
It extracts and visualizes monthly pairing PDFs (final or prelim) into structured, searchable tables — optimized for iPad Pro and desktop browsers.

Current version: `v0.1.0`

---

## 🌐 Live Demo

Visit [https://pairingviewer.com](https://pairingviewer.com)

---

## 🚀 Features

- 📄 Upload airline pairing PDF (supports both **Final** and **Prelim**)
- ⚡ Fast, parallelized PDF-to-text extraction
- 🧠 Smart parser: detects TAFB, per diem, layovers, report/release times, and more
- 📱 Optimized UI for **iPad Pro M4 landscape**
- 🌙 Night mode + persistent column layout with Tabulator
- 🔍 Instant search, filter by redeye, commutable, lazy, weekdays, etc.

---

## 🏗️ Architecture

| Layer | Stack |
|-------|--------|
| Frontend | HTML5 + Tabulator 5.x + Vanilla JS |
| Backend | Flask (Python 3.11+) + PyMuPDF |
| Hosting | Any VPS (Nginx + Gunicorn + Certbot) |

---

## 📦 Repository Docs

- [CHANGELOG.md](CHANGELOG.md)
- [CONTRIBUTING.md](CONTRIBUTING.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- [SECURITY.md](SECURITY.md)
- [RELEASE.md](RELEASE.md)
