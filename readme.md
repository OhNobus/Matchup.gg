Technology:

- Python 3
- PySide6
- Qt Widgets
- No web technologies
- No server
- No database

Storage:

- Matchups are Markdown files.
- Folder structure: data/<champion></champion>/<opponent></opponent>.md
- overview.md contains champion overview.
- YAML frontmatter stores metadata.
- Never store matchup content in source code.

UI:

- Main window contains search bar.
- Main content consists of matchup tiles.
- Clicking a tile opens a dialog.
- Dialog renders Markdown.
- Matchups can be edited from the dialog.

Architecture:

- UI and storage must remain separate.
- Keep dependencies minimal.
- Application must work with a configurable NAS data directory.




# LoL Matchup Tool

Anwendung zum schnellen Abrufen und Bearbeiten eigener
League-of-Legends-Matchup-Notizen.

## Hauptziele

- Matchups innerhalb weniger Sekunden finden
- Inhalte übersichtlich darstellen
- Inhalte direkt in der Anwendung bearbeiten
- Markdown als Contentformat
- Schutz vor versehentlichem Datenverlust
- späterer Betrieb auf eigener Server-/NAS-Infrastruktur
