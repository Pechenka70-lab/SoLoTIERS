# SoLoTIERS — Render-ready package

This package contains the compiled SoLoTIERS React frontend and the Flask API in one service.

## Render settings
- Runtime: Python
- Build Command: `pip install -r requirements.txt`
- Start Command: `gunicorn --bind 0.0.0.0:$PORT backend.app:app`

## Required environment variables
- `SECRET_KEY` — long random secret
- `DISCORD_API_KEY` — the same key used by the Discord bot
- `ADMIN_USERNAME` — optional
- `ADMIN_PASSWORD` — optional
- `DATABASE_PATH` — optional; defaults to `data/solotiers.sqlite3`

The frontend is served by the Flask app from `frontend/`.
