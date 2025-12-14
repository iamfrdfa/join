# Join — Kanban Board

**Join** ist ein web-basiertes **Kanban Board**, mit dem Aufgaben übersichtlich organisiert und entlang eines klaren Workflows bewegt werden können.  
Der Fokus liegt auf einem schnellen, verständlichen UI und einem soliden Setup für **User-Management** und **Authentifizierung**.

---

## Features

- **Kanban Workflow**: Aufgaben von *To Do* → *In Progress* → *Awaiting Feedback* → *Done*
- **Drag & Drop**: Tasks intuitiv zwischen Spalten verschieben
- **Task-Management**: Aufgaben anlegen, bearbeiten und löschen (Titel, Beschreibung, Kategorie, Priorität, Fälligkeitsdatum)
- **User & Auth**: Registrierung/Login, Sessions und geschützter Zugriff auf Inhalte
- **Datenpersistenz**
    - **Firebase** für Speicherung und Synchronisation
    - **LocalStorage** für lokale Zustände/Cache (z.B. Session, UI-State – je nach Implementierung)
- **Responsive UI**: Nutzbar auf Desktop und Mobile

> Nicht enthalten (bewusst): Suche, Filter, Subtasks.

---

## Screenshots

> Füge hier 2–4 Screenshots ein (Board, Task-Dialog, Login, Mobile-Ansicht).
>
> Beispiel:
> - `./assets/board.png`
> - `./assets/task-detail.png`
> - `./assets/login.png`
> - `./assets/mobile.png`

---

## Live Demo

- Demo: **(Link hier einfügen)**
- Repository: **(GitHub Link hier einfügen)**

---

## Tech Stack

- **HTML / CSS / JavaScript**
- **Firebase** (Auth + Database/Storage je nach Setup)
- **LocalStorage** (Session/Cache/UI-State)

---

## Getting Started

### Voraussetzungen

- Ein moderner Browser
- Node.js (falls dein Build/Dev-Setup darüber läuft)

### Lokales Setup

```bash
# Repo klonen
git clone https://github.com/<dein-user>/<dein-repo>.git

# Öffnen
cd <dein-repo>
