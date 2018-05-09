# Sentinel Website demo

## Install

You should install python3 and [Django](https://www.djangoproject.com/).
Please follow the [instruction](https://docs.djangoproject.com/en/2.0/intro/install/) to install Django.

## Install Dependencies

You need to install django-rest-framework package.
Make sure you're using python version 3. If you have both versions in your system, indicate explicitly by using 'pip3' instead of just 'pip'.
```
$ sudo pip install django-rest-framework
```

## Start Server

Initialize database according to the schema that you defined with models.

Make sure you're using python version 3. If you have both versions, indicate explicitly by using 'python3' instead of just 'python'.

```
$ cd uppsala
$ python manager.py migrate
$ python manager.py runserver
```

The server will be running on localhost:8000

You can also expose your server by binding '0.0.0.0'

```
$ python manager.py runserver 0.0.0.0:80
```

## Administration

Create the first admin user.

```
$ python manager.py createsuperuser
```

You can view all of the records on http://localhost:8000/admin. Log in with the superuser's account you've jsut made.

Please refer to Django's official documentation for further development.
