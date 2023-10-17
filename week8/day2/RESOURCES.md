# Resources

## General

- [Redmonk: Postgres: the next generation. Investing in the next generation of committers.](https://redmonk.com/jgovernor/2023/10/10/postgres-the-next-generation-investing-in-the-next-generation-of-committers/)
- [Things I wish someone would have told me about configuring VSCode](https://www.bryanbraun.com/2023/08/10/things-i-wish-someone-would-have-told-me-about-configuring-vscode/)

## Django Rest Framework

- [Stack Overflow: Difference between Django and Django rest framework](https://stackoverflow.com/a/68113903)
- [Log Rocket:How to create a REST API with Django REST framework](https://blog.logrocket.com/django-rest-framework-create-api/)

## What's the deal with `pyenv`?

- [Python: Creating a clean learning environment with pyenv, pyenv-virtualenv & pipX](https://towardsdatascience.com/python-how-to-create-a-clean-learning-environment-with-pyenv-pyenv-virtualenv-pipx-ed17fbd9b790)

### What does it do?

Essentially, `pyenv` is to Python what `nvm` is to NodeJS (kinda).

(credit to Google's Bard for the following summaries)

> In the simplest terms, `pyenv` is a tool that helps you manage multiple versions of Python on your computer. It allows you to install, uninstall, and switch between different Python versions easily. This is particularly useful for developers who work on projects that require specific Python versions or for those who want to experiment with different Python features without affecting their system's default Python installation.
>
> Think of `pyenv` as a personal Python version manager that keeps track of all the Python versions you have installed and lets you choose which one to use for a particular task or project.

### Setting it up

> The `env/bin/activate` script is used to activate a specific Python virtual environment, ensuring that the correct Python version and associated packages are used for your project.
>
> It modifies your current shell session to use the Python environment located in the `env` directory.
>
> Consider it like entering a specific workspace for your project, where you have all the necessary tools and configurations readily available.
> ...

#### Activating an environment

> The `env` directory is specifically created when you create a Python virtual environment using tools like `virtualenv` or `pyenv`.
>
> Once the `env` directory is created, you can activate the virtual environment using the `env/bin/activate` script.

### What does `python -m venv env` actually do?

#### Breaking down the command

- `-m`: The `m` flag indicates that a module is being executed as a script.
- `venv`: This is the name of the module responsible for creating virtual environments.
- `env`: This is the name of the directory where the virtual environment will be created.

#### Steps to use the command

1. Execute the following command in your project folder to create a directory named `env` containing the virtual environment setup.

    ```bash
    python -m venv env
    ```

2. To activate the virtual environment, use the following command:

    ```bash
    source env/bin/activate
    ```

3. Once activated, the virtual environment's Python interpreter and packages will be used for any Python commands executed in that terminal session.
4. To deactivate the virtual environment, simply type:

    ```bash
    deactivate
    ```

This will revert to using the system's default Python environment.
