## Dependencies
* Python3+
* Node
* PostgreSQL

## Getting Started
### Installation
Clone this repository:

    git clone 

Create virtualenv and install all requirements in **backend** directory:

    cd elvedin/backend/
    python -m venv venv_name
    .venv_name\scripts\activate
    pip install -r requirements.txt

Install all needed node_modules in **frontend** directory:

    cd elvedin/frontend/
    npm install

Prepare database in postgreSQL


Set up database connection in **elvedin/backend/backend/settings.py** in DATABASES section:

    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql_psycopg2',
            'NAME': 'shop',
            'USER': 'YOUR_USERNAME', # replace with your own username
            'PASSWORD': 'YOUR_PASSWORD', # replace with your own password
            'HOST': 'localhost',
            'PORT': ''
        }
    }

Fire up **backend** server:

    cd elvedin/backend/
    python manage.py migrate
    python manage.py runserver

Open another terminal for **frontend** server:

    cd elvedin/frontend/
    npm start

## Built With
* [React](https://facebook.github.io/react/) - A JavaScript library for building UI
* [Semantic UI React](https://react.semantic-ui.com/introduction) - A React UI framework
* [Redux](https://redux.js.org/) - A predictable state container for JavaScript apps
* [Django REST framework](http://www.django-rest-framework.org/) - A powerful and flexible toolkit for building Web APIs
* [django-rest-framework-jwt](http://getblimp.github.io/django-rest-framework-jwt/) - JSON Web Token Authentication support for Django REST framework
* [axios](https://github.com/mzabriskie/axios) - A Promised based HTTP client
* [toastr](https://github.com/CodeSeven/toastr) - Simple javascript toast notifications


