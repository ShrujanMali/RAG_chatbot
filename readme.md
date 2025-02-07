# Chat Website with Django and Django Channels

This tutorial will guide you through creating a chat website using Django and Django Channels.

## Getting Started

### 1. Setting up a Django Project

1. Create and enter the desired directory for project setup.

2. Create a virtual environment using pipenv or other means:

    ```shell
    pipenv shell
    ```

3. Install Django:

    ```shell
    pip install django
    ```

4. Create a Django project called ChatPrj:

    ```shell
    django-admin startproject ChatPrj
    ```

5. Create an app called ChatApp:

    ```shell
    python manage.py startapp ChatApp
    ```

6. Open the project in your code editor.

7. Create a templates folder and register it in the project's settings.

8. Register the app in the project's settings.

9. Create URLs for the app and register them in the project's URLs.

### 2. Installing Libraries

1. Install Django Channels:

    ```shell
    pip install django-channels
    ```

2. Install Daphne:

    ```shell
    pip install daphne
    ```
3. Add  ChatApp, daphne and channels to `installed_apps` in `settings.py` file: 
    ```python
    INSTALLED_APPS = [
        'daphne',
        'django.contrib.admin',
        'django.contrib.auth',
        'django.contrib.contenttypes',
        'django.contrib.sessions',
        'django.contrib.messages',
        'django.contrib.staticfiles',
        'ChatApp',
        'channels',
    ]
    ```
