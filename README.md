# DA Notes Backend 📝

[English Version](#english-version) | [Deutsche Version](#deutsche-version)

---

<a name="english-version"></a>
## 🇺🇸 English Version

This repository contains the backend for the DA Notes app. It uses the Django REST Framework (DRF) to provide a robust API for the Angular frontend.

###Features
* Full CRUD (Create, Read, Update, Delete) functionality.
* Support for Favorites (marked) and Trash (trash) statuses.
* Pre-configured CORS settings for local Angular development (localhost:4200).

### Installation & Setup
Execute these commands in your terminal:

1. **Create & activate virtual environment:**
```bash
python -m venv venv
# Windows:
.\venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

2. **Install dependencies:**
```bash
pip install django djangorestframework django-cors-headers
```

3. **Run database migrations:**
```bash
python manage.py makemigrations
python manage.py migrate
```

4. **Start the server:**
```bash
python manage.py runserver
```

The API is now accessible at http://127.0.0.1.

---

### API Reference

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/notes/` | List all notes |
| `POST` | `/notes/` | Create a new note |
| `PATCH` | `/notes/{id}/` | Update an existing note (e.g., mark as favorite) |
| `DELETE` | `/notes/{id}/` | Permanently delete a note |

---

<a name="deutsche-version"></a>
## 🇩🇪 Deutsche Version

Dieses Repository enthält das Backend für die **DA Notes** App der Developer Akademie. Es basiert auf dem **Django REST Framework (DRF)** und dient als API für das Angular-Frontend.

### Funktionen
* Vollständiges **CRUD** (Erstellen, Lesen, Bearbeiten, Löschen) für Notizen.
* Unterstützung für **Favoriten** (`marked`) und **Papierkorb** (`trash`).
* Vorkonfiguriertes **CORS** für die Kommunikation mit Angular (`localhost:4200`).

### Installation & Setup

Führe diese Befehle nacheinander in deinem Terminal aus:

1. **Virtuelle Umgebung erstellen & aktivieren:**
```bash
python -m venv venv
# Windows:
.\venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

2. **Abhängigkeiten installieren:**
```bash
pip install django djangorestframework django-cors-headers
```

3. **Datenbank-Migrationen durchführen:**
```bash
python manage.py makemigrations
python manage.py migrate
```

4. **Server starten**
```bash
python manage.py runserver
```

Die API ist nun unter http://127.0.0.1 erreichbar.

---

### API Endpoints (Übersicht)

| Methode | Endpunkt | Beschreibung |
| :--- | :--- | :--- |
| `GET` | `/notes/` | Alle Notizen abrufen / List all notes |
| `POST` | `/notes/` | Neue Notiz erstellen / Create new note |
| `PATCH` | `/notes/{id}/` | Notiz aktualisieren (z.B. Favorit) / Update note |
| `DELETE` | `/notes/{id}/` | Notiz endgültig löschen / Delete note |
