# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 31: Django REST Framework & Docker

Docker is really just Linux containers which are a type of virtualization.

What’s the downside to a virtual machine? Size and speed. A typical guest operating system can easily take up 700MB of size. So if one physical server supports three virtual machines, that’s at least 2.1GB of disk space taken up along with separate needs for CPU and memory resources.

Docker is a way to implement Linux containers.

Virtual Machines are like homes: stand-alone buildings with their own infrastructure including plumbing and heating, as well as a kitchen, bathrooms, bedrooms, and so on. Docker containers are like apartments: they share common infrastructure like plumbing and heating, but come in various sizes that match the exact needs of an owner.

Containers vs Virtual Environments

Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

## Django for APIs

Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

Read more on the following link

[Django for APIs](https://djangoforapis.com/library-website-and-api/)



...............................................................................

__Attributions for the following Reference materials and their authors__

[A beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

[Django for APIs](https://djangoforapis.com/library-website-and-api/)

[>> NEXT (Read: Class 32)](https://wondwosentsige.github.io/code-401-reading-note/class-32)