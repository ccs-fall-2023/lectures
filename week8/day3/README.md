# Week 8 - Day 3

Time for REST! (not _a_ rest, but Representational State Transfer)

## Hour 1

Show'n'Tell'n'Debug

## Hour 2-3

Let's build the Apple CEOs app, but this time as an API.

Also, we're gonna get _CRUDdy_!

## Helpful Resources

What the heck is "serialization??"

It's basically a way for the Django REST Framework to convert your data into JSON or XML that can be sent as a `response` from your API. The inverse, deserialization, takes place when the framework needs to convert `requests` into something Python understands.

* [Django REST Framework Quickstart](https://www.django-rest-framework.org/tutorial/quickstart/#project-setup)

Isaac recommended using this to manage installs, it looks like it's much easier than jumping through `pip` and `pyenv` separately.

* [Pipenv](https://pypi.org/project/pipenv/)