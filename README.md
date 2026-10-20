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

## Testing

```sh
python manage.py test polls
```

Tests are in `polls/tests.py`. They cover `Question.was_published_recently()` and the index and detail views, including that future questions stay hidden.

Run one test class or method:

```sh
python manage.py test polls.tests.QuestionIndexViewTests
python manage.py test polls.tests.QuestionModelTests.test_was_published_recently_with_future_question
```
