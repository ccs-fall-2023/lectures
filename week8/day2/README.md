# Week 8 - Day 2

Today we're going to break down the [Django Tutorial from MDN](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Tutorial_local_library_website).

## Common Steps, a Review

Start with:

```python
pip install django
django-admin startproject [YOUR_PROJECT_NAME]
cd [YOUR_PROJECT_NAME]
```

Run the server for your project:

```python
python manage.py runserver
```

Create your web apps in the current directory:

```python
python manage.py startapp [YOUR_APP_NAME]
```

_Working with `pyenv` here would also be handy! There's more information about that [here](./RESOURCES.md#whats-the-deal-with-pyenv)._

## Resources

* [Django Rest Framework](https://www.django-rest-framework.org/)
* [Django Docs: PostgreSQL notes](https://docs.djangoproject.com/en/4.2/ref/databases/#postgresql-notes)

### What's the differnce in a project and an app?

* [Project VS App in Django](https://atufashireen.medium.com/project-vs-app-in-django-755cf2a82312)

> A _project_ refers to the entire application and all its parts.
>
> An _app _refers to a submodule of the project. It’s self-sufficient and not intertwined with the other apps in the project [...] An app typically has its own `models.py`` (which might actually be empty). [...] A simple project might only have one app.

### Using `requirements.txt`, it's like `package.json` but with 🐍🐍🐍

* [LearnPython.org: The Python Requirements File and How to Create it](https://learnpython.com/blog/python-requirements-file/)
* [How to install Python packages with pip and requirements.txt](https://note.nkmk.me/en/python-pip-install-requirements/)
