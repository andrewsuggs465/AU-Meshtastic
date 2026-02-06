# Instructions for compilation:
- clone the repository and import into vscode
- python3 -m venv venv
- source venv/bin/activate
- pip install mkdocs
- mkdocs gh-deploy -f mkdocs.yml --clean
- or mkdocs serve -f mkdocs.yml locally
# Events
index.md
# Events

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
---
title: 2026-02-12 — Weekly Build Night
date: 2026-02-12 18:00 CST
location: SPARC Lab (MEB 123)
organizer: spectralstrider
---

# 2026-02-12 — Weekly Build Night *EXAMPLE*

- **Time:** 18:00 — 20:00
- **Location:** SPARC Lab (MEB 123)
- **Organizer:** spectralstrider

Join us for a hands-on session focused on flashing firmware, assembling WisBlock nodes, and introductory RF topics. Bring your device or just come to learn.
