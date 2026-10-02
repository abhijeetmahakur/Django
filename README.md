# Django Blog Starter

This repository is an early Django project scaffold. It defines a `Post` model and enables Django's admin, but the current URL configuration only exposes `/admin/`; there are no public blog views or routes yet.

## Requirements

- Python 3.12 or newer
- Django 6.0.2 (pinned in `requirements.txt`)

## Setup and run

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python manage.py check
python manage.py runserver
```

The project admin is available at <http://127.0.0.1:8000/admin/>. Create a local administrator with `python manage.py createsuperuser` if needed.

## Project structure

- `manage.py` is the Django command-line entry point.
- `myproject/` contains settings and URL configuration.
- `blog/models.py` defines the post data model.
- `blog/tests.py` is currently an empty test placeholder.

## Security and data notes

This is a development scaffold, not a production deployment. The checked-in settings use development security configuration; do not expose the server publicly until the signing key, debug mode, and allowed hosts are configured safely. A SQLite database is currently tracked in the repository. The `.gitignore` prevents newly created local databases from being added, but does not untrack that existing file.

## License

No project license is included. Confirm code and tutorial provenance before choosing one or granting reuse rights.