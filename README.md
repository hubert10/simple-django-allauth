---
noteId: "a7ae8fb0da5211eabcc5fb5636741ef8"
tags: []
---

# Simple Django AllAuth Example

This simple project integrates django-allauth module for local authentication and shows how you can write custom adapters for social authentication. By default, the allauth module does not automatically authenticate users already having accounts on backend, and trying to register with social authentication, so I have included an adapter to handle this issue.
This app can be run using docker.

###### WARNING! This simple project is only for local testing, it's not prepared for social authentication into remote server.

## Prerequisites

- Docker
- Docker-compose

## Getting Started

Steps to build, and run project:

1. `cd` to root of project
2. `docker-compose build`
3. `docker-compose up`
4. `docker-compose exec web python manage.py makemigrations`
5. `docker-compose exec web python manage.py migrate`
6. `docker-compose exec web python manage.py createsuperuser`

To test signup on browser, go to:

## Examples of usage

`http://localhost:8000/accounts/signup/`
for signup:

## Links

Check out official documentation to this project:
https://django-allauth.readthedocs.io/en/latest/installation.html
