FROM python:alpine

WORKDIR /usr/app

RUN pip install django
RUN pip install djangorestframework

RUN django-admin startproject backend .

WORKDIR /usr/app/backend

RUN django-admin startapp quickstart

WORKDIR /usr/app

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]