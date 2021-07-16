# api_wine

### Shop API

## Table of contents

-   [General info](#general-info)
-   [Features](#features)
-   [API Endpoints](#api-endpoints)
-   [Technologies](#technologies)
-   [Setup](#setup)

## General info<a name="general-info"></a>

Shop API is a REST API built with Flask & SQLAlchemy to operate CRUD operation on the database. The different routes are described below in the API Endpoint section.

## Features<a name="features"></a>

### User features

-   Allow user to create an account
-   Allow user to login
-   Allow user to disconnect
-   Allow user to save information in the database
-   Allow the user to update or delete their information (name, password, address, etc…)
-   Allow user to delete their account
-   Allow user to reset their password through Email
-   Allow user to upload a profile picture
-   Allow user to save setting in the database
-   Allow user to update or delete their settings (theme, default currency)

## API Endpoints<a name="api-endpoints"></a>

After running the server, consult Documentation at :

> http://127.0.0.1:5000/

-   Product
    -   Return JSON with all products
    -   Return JSON selected product

Database schema:

![DB Screenshot](https://github.com/antoineratat/api_shop/blob/master/screenshots/1.png?raw=true)

## Technologies<a name="technologies"></a>

Project is created with:

-   python V3.9.0
-   astroid V2.4.2
-   bcrypt V3.2.0
-   blinker V1.4
-   certifi V2020.12.5
-   cffi V1.14.4
-   chardet V4.0.0
-   click V7.1.2
-   colorama V0.4.4
-   Flask V1.1.2
-   Flask-Bcrypt V0.7.1
-   Flask-Cors V3.0.9
-   Flask-JWT-Extended V3.25.0
-   Flask-Mail V0.9.1
-   Flask-SQLAlchemy V2.4.4
-   gunicorn V20.0.4
-   idna V2.10
-   isort V5.6.4
-   itsdangerous V1.1.0
-   Jinja2 V2.11.2
-   lazy-object-proxy V1.4.3
-   MarkupSafe V1.1.1
-   mccabe V0.6.1
-   psycopg2 V2.8.6
-   pycparser V2.20
-   PyJWT V1.7.1
-   pylint V2.6.0
-   requests V2.25.1
-   six V1.15.0
-   SQLAlchemy V1.3.20
-   stripe V2.55.1
-   toml V0.10.2
-   urllib3 V1.26.2
-   Werkzeug V1.0.1
-   wrapt V1.12.1

## Setup<a name="setup"></a>

### Import project

```
$ git clone https://github.com/antoineratat/api_wine.git
$ py -3 -m venv venv
$ venv\Script\Activate
$ cd wine_api
$ pip install -r requirements.txt
```

### Create Environnement Variable

```
$ SECRET_KEY = '12345678912345678912345678912312'
$ DATABASE_URL = 'postgres://myurl:port/dbname'
```

### Initialize Database

```
$ venv\Script\Activate
$ python
$ from run import db
$ db.create_all()
$ exit()
```

### Run project

```
$ python run.py
```
