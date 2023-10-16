# Django in 7 Simple Steps

Steps taken from the [_Django vs Fast API: A Detailed Comparison_ article](https://medium.com/@ShortHills_Tech/django-vs-fast-api-a-detailed-comparison-df8d00f3c3b2)

1. Install Django

    ```python
    pip install django
    ```

2. Create a Project (replace `YOUR_PROJECT_NAME` with an actual project name)

    ```python
    django-admin startproject [YOUR_PROJECT_NAME]
    ```

3. Now, change into your project directory

    ```python
    cd [YOUR_PROJECT_NAME]
    ```

4. Run the server with the default Django homepage.

    ```python
    python manage.py runserver
    ```

5. Now you can create your web apps in the current directory([YOUR_PROJECT_NAME]). To create an app use this command:

    ```python
    python manage.py startapp [YOUR_APP_NAME]
    ```

## Helpful commands

Check your Django version

```python
python -m django —-version
```

Check which django commands are available

```python
django-admin
```
