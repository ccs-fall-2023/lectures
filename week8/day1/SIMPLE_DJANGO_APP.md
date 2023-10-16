# Django in 7 Simple Steps

Steps taken from the [_Django vs Fast API: A Detailed Comparison_ article](https://medium.com/@ShortHills_Tech/django-vs-fast-api-a-detailed-comparison-df8d00f3c3b2)

1. Install Django

    ```python
    pip install django
    ```

2. Check version

    ```python
    python -m django — version
    ```

3. To check which django commands are available

    ```python
    django-admin
    ```

4. Create a Project

    ```python
    django-admin startproject hello_world_app
    ```

5. Now, move to Project Directory

    ```python
    cd hello_world_app
    ```

6. Run the server with the default Django homepage.

    ```python
    python manage.py runserver
    ```

7. Now you can create your web apps in the current directory(hello_world_app). To create an app use this command:

    ```python
    python manage.py startapp APP_NAME
    ```