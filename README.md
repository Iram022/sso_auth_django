Django SSO Authentication with Google Login

This project implements Single Sign-On (SSO) authentication in Django using Google OAuth via the `django-allauth` library.

Features

Login with Google (OAuth2)
Secure authentication using Django Allauth
REST-ready setup
Tested on `localhost:8000`


Installation

1. Clone the repo:
   git clone https://github.com/your-username/sso-auth-django.git
   cd sso-auth-django

2. Create a virtual Environment:
    python -m venv venv
    venv\Scripts\activate  

3. Install dependencies
    pip install -r requirements.txt

4. Run migrations
    python manage.py makemigrations
    python manage.py migrate

5. Create superuser
    python manage.py createsuperuser
    (username : iramsiddiqui | password: ******)

6. Start the development server
    python manage.py runserver


## Google OAuth Setup

1. Go to Google Cloud Console

2. Create a project and set up OAuth 2.0 credentials

3. Set the redirect URI to:
    http://localhost:8000/accounts/google/login/callback/
    
4. Copy your Client ID and Secret, and paste them in the Django admin    panel under Social Applications.


## URLS:
1. Login: http://localhost:8000/accounts/login/

2. Admin: http://localhost:8000/admin/

