### Creating virtual environment for python (To isolate different projects)
*Installing virtual environment globally*

    pip install virtualenv
*Creating virtual environment*

    virtualenv venv
*Activate virtual environment 'env1'*

    env1/Scripts/activate

*If execution policy is restricted* 

    Get-ExecutionPolicy
    Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
    Get-ExecutionPolicy
    

### Django commands 
*Installing Django*

    pip install Django

*Creating a project folder and initing Django inside* 

    django-admin startproject ecommerce

*Run the manage.py file inside project repo to run Django server*

    python manage.py runserver

*Creatig a Django app (python package) within a project*

    django-admin startapp store

1. Add this app name to INSTALLED_APPS in settings.py 
2. Define models for the app in models.py

*Creating migrations package*

    python manage.py makemigrations

*Performing migrations*

    python manage.py migrate

3. Static files path in settings

STATICFILES_DIRS = [BASE_DIR/'static']

MEDIA_ROOT = [BASE_DIR/'static/media']

*Creating super user for djangio admin*

    python manage.py createsuperuser
