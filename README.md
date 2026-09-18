# Join — Kanban Board

**Join** ist ein web-basiertes **Kanban Board**, mit dem Aufgaben übersichtlich organisiert und entlang eines klaren Workflows bewegt werden können.
Der Fokus liegt auf einem schnellen, verständlichen UI mit Drag & Drop, Kontaktverwaltung und einer einfachen Registrierung/Anmeldung.

---

## Features

- **Kanban Workflow**: Aufgaben von *To Do* → *In Progress* → *Awaiting Feedback* → *Done*
- **Drag & Drop**: Tasks intuitiv zwischen Spalten verschieben
- **Task-Management**: Aufgaben anlegen, bearbeiten und löschen (Titel, Beschreibung, Kategorie, Priorität, Fälligkeitsdatum, Subtasks)
- **Kontaktverwaltung**: Kontakte anlegen, bearbeiten, löschen und Tasks zuweisen
- **Dashboard**: Übersicht über anstehende und dringende Aufgaben auf der Summary-Seite
- **Registrierung & Login**: eigener Account oder Gast-Zugang
- **Datenpersistenz**: Firebase Realtime Database für Tasks, Kontakte und Nutzerdaten
- **Responsive UI**: Nutzbar auf Desktop und Mobile

---

## Tech Stack

- **HTML / CSS / JavaScript** (Vanilla, ohne Framework)
- **Firebase Realtime Database** als Backend für Tasks, Kontakte und Nutzer
- **LocalStorage** für UI-/Session-Zustand im Browser

---

## Projektstruktur

```
join/
├── index.html          # Summary / Dashboard
├── board.html           # Kanban Board
├── add_task.html        # Task anlegen
├── contacts.html         # Kontaktverwaltung
├── login.html / register.html
├── legal.html / privacy.html / help.html
├── js/                   # Anwendungslogik (Board, Tasks, Kontakte, Auth, Templates)
├── templates/            # wiederverwendbare HTML-Bausteine (Header, Sidebar, Mobile-Menü)
├── assets/ / img/        # Icons und statische Assets
```

---

## Getting Started

### Voraussetzungen

- Ein moderner Browser
- Ein lokaler Webserver (z. B. die VS-Code-Extension "Live Server"), da einige Seiten Inhalte per `fetch()` nachladen und daher nicht zuverlässig direkt über `file://` funktionieren

### Lokales Setup

```bash
# Repo klonen
git clone git@github.com:iamfrdfa/join.git

# Öffnen
cd join

# mit einem lokalen Server starten, z. B.
npx serve .
```

Anschließend `index.html` (bzw. `login.html`) im Browser aufrufen.

---

## Bekannte Einschränkungen

- Die Firebase-Datenbank ist derzeit ohne serverseitige Security Rules / echte Authentifizierung angebunden — Login und Zugriffskontrolle laufen ausschließlich clientseitig. Für einen produktiven Einsatz sollten Firebase Auth und passende Security Rules ergänzt werden.
- Keine Such- oder Filterfunktion für Tasks.

---

## Repository

<https://github.com/iamfrdfa/join>
