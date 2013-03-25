pinax-project-social-allauth
============================

a starter project for social components based on pinax-project-social (https://github.com/pinax/pinax-project-social/) that adds social authentication login and registration including django-allauth. More info about django-allauth can be found in the (allauth official repository)[https://github.com/pennersr/django-allauth/]

Example usage
=============

    $ virtualenv mysite
    $ source mysite/bin/activate
    (mysite)$ pip install Django==1.4.5
    (mysite)$ django-admin.py startproject --template=https://github.com/danfreak/pinax-project-social-allauth/zipball/master mysite
    (mysite)$ cd mysite
    (mysite)$ pip install -r requirements.txt
    (mysite)$ python manage.py syncdb
    (mysite)$ python manage.py runserver

Hit http://127.0.0.1:8000 to view the site!

To enable the social login/signup feature uncomment the providers you are interested in the [settings.py](https://github.com/danfreak/pinax-project-social-allauth/blob/master/project_name/settings.py#L143) file. You should then login into your project admin backend at http://127.0.0.1:8000/admin and setup 

An extensive guide about setting up providers can be found on the [django-allauth page](https://github.com/pennersr/django-allauth#providers)

What's included
===============

 * user profiles which are hooked up to the sign up process
 * django-allauth for social authentication and registration (https://github.com/pennersr/django-allauth/)
