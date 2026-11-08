# Laboratory Activity 9: System-to-System Integration

Flask + SQLite student app. View, save, send and retrieve records with a partner's API.

## Run locally
    pip install -r requirements.txt
    python init_db.py
    python app.py

## Render
- Build: `pip install -r requirements.txt`  Start: `gunicorn app:app`

## Endpoints
- `GET/POST /api/students`, `GET/PUT/DELETE /api/students/<id>` — local records
- `GET /partner-records?url=` — fetch partner records (HTTPS `*.onrender.com/api/students` only)
- `POST /import-student` — save a partner record, source `Classmate API`
- `POST /send-to-partner` — send a practice record to the partner

Use fictional data only.
