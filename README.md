# django_official_tutorial

Polls app built while following the [official Django tutorial](https://docs.djangoproject.com/en/stable/intro/tutorial01/).

## Run

```sh
python -m venv .venv && source .venv/bin/activate
pip install django
python manage.py migrate
python manage.py runserver
```

Set `DJANGO_SECRET_KEY` in the environment for any non-local use.
