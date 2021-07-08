# About Project
This is a marketplace store where users can register on the site and sell products.
<br>
This project generated by restfull architecture with django.
<br>
## Tech:
1. Python
2. Django
3. Django-Rest-Framework
4. Rabbitmq
5. Redis
6. Celery
7. Celery beat
<br>

## Installation:

### Clone Project
```
$ git clone https://github.com/rahmanipy/restful-django-shop.git
```
### Create venv and activate
```
$ python3 -m venv venv
$ python3 venv/bin/activate
```
### Install Requirements.txt
```
$ pip install -r requirements.txt
```
### Start Rabbitmq
```
$ sudo systemctl start rabbitmq-server
```
### Start Redis
```
$ sudo systemctl start redis
```
### Start Celery
```
$ celery -A DrfShop worker -l INFO
```
### Start Celery Beat
```
$ celery -A DrfShop beat -l INFO --scheduler django_celery_beat.schedulers:DatabaseScheduler
```
### Run Project
```
$ python manage.py runserver
```
<br>
Now project is up on :  localhost:8000/
