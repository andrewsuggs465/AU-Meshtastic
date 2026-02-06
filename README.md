# Auburn University Meshtastic

A student-led community exploring Meshtastic, LoRa, and mesh networking at Auburn University.

## Quick Start

### Setup

1. Clone the repository and open in VS Code.
2. Create and activate a Python virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install mkdocs mkdocs-material pymdown-extensions
   ```

4. Serve the docs locally:

   ```bash
   mkdocs serve
   ```

   Then open <http://127.0.0.1:8000>

### Deployment

Deploy to GitHub Pages:

```bash

mkdocs gh-deploy -f mkdocs.yml --clean
```

## Events

index.md

This page lists upcoming meetings, workshops, and social events. Add each event as a separate markdown file under `docs/events/` so it appears as its own module.

## Upcoming

- [2026-02-12 — Weekly Build Night](2026-02-12-weekly-build-night.md) — 18:00 — SPARC Lab

---

## How to add an event

1. Create a file at `docs/events/YYYY-MM-DD-slug.md`.
2. Add a short frontmatter block (optional) followed by details.
3. Update `docs/events/index.md` to link to the new event.

Example filename: `docs/events/2026-03-01-kickoff.md`.

2026-02-12-weekly-build-night.md

\# 2026-02-12 — Weekly Build Night *EXAMPLE*

- **Time:** 18:00 — 20:00
- **Location:** SPARC Lab (MEB 123)
- **Organizer:** Andrew

Join us for a hands-on session focused on flashing firmware, assembling WisBlock nodes, and introductory RF topics. Bring your device or just come to learn.
