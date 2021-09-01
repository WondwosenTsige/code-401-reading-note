# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 29: Custom User Model

Django comes up with a built-in User model for authentication.

Setup
To start, create a new Django project from the command line. We need to do several things:

create and navigate into a dedicated directory called accounts for our code
install Django
make a new Django project called config
make a new app accounts
start the local web server

Here are the commands to run:

$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver












...............................................................................

__Attributions for the following Reference materials and their authors__

[Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

[DjangoX](https://github.com/wsvincent/djangox)

[>> NEXT (Read: Class 30)](https://wondwosentsige.github.io/code-401-reading-note/class-30)