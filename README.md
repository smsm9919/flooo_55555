
# AutoMarket Minimal — Render Ready

## Structure
- `app.py` — Flask entrypoint
- `gunicorn.conf.py` — Gunicorn config
- `requirements.txt`
- `render.yaml` — Render Blueprint definition
- `templates/` and `static/` — frontend assets
- `models.py` and `i18n.py` — application modules

## Deploy on Render
1. Push these files directly to your GitHub repo **root** (main branch).
2. In Render: New → Blueprint → select the repo.
3. Render will auto-detect `render.yaml` and create:
   - Web Service: automarket
   - PostgreSQL: automarket-db

## Verify
- `/healthz` endpoint returns healthy status.
- `/db-ping` checks database connectivity.
