# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 19: Django Models

Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc

Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data.

In order to log into the admin site, we need a user account with Staff status enabled. In order to view and create records we also need this user to have permissions to manage all our objects.  You can create a "superuser" account that has full access to the site and all needed permissions using manage.py.

Call the following command, in the same directory as manage.py, to create the superuser. You will be prompted to enter a username, email address, and strong password.

    python3 manage.py createsuperuser

needs to read more on the following resources 

[A Complete Beginner's Guide to Django - Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)

[A Complete Beginner's Guide to Django - Part 2](https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html)

.....










...............................................................................

__Attributions for the following Reference materials and their authors__

[Using Models: Django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)

[Django admin site](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

[>> NEXT (Read: Class 28)](https://wondwosentsige.github.io/code-401-reading-note/class-28)