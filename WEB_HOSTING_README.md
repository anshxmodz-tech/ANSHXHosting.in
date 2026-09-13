# ANSH HOSTING – Web + Bot Hosting

Supported deployments:
- Python bot: `main.py` + `requirements.txt`
- Python web app: `app.py` (Flask apps are started with an isolated localhost port)
- PHP website: `index.php` (requires PHP installed on the host)
- Static website: `index.html`
- ZIP uploads: multiple files/folders are supported.

Public URL formats:
- Static: `/host/<server_id>/`
- PHP/Python web app: `/app/<server_id>/`

For Python web apps, use the `PORT` environment variable when your framework needs a port:
`PORT = int(os.environ.get("PORT", 5000))`

The hosting panel automatically detects `app.py`, `index.php`, or `index.html` in an uploaded ZIP.
