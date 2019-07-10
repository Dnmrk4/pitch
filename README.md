# [INIT PITCH](https://pitch-es.herokuapp.com/)

### Author

By [Danmark Mutai](https://github.com/Dnmrk4)

## Description

- This is a web application made for users to post pitches on any of the 4 different categories. These categories are:

    1. Pickup lines
    2. Promotion
    3. Product
    4. Interview 

- A user that is reading the pitches can give feedback to the pitch posts by commenting, liking or disliking the pitch. 

#### Date: JUL 2nd, 2019

## BDD

Get the specifications by clicking [here](/specs.md)

## Setup

#### - Requirements

- You need to have python 3.6 installed in your computer.
- You must have a working internet service.
- 

#### - Setup and Instalations

- You first need to clone the application by runing the following command on the terminal:
`$ git clone https://github.com/Dnmrk4/pitch.git && cd pitch` then install [Postgres](https://www.postgresql.org/download/) to your computer.

- Run the following commands in the same terminal:
`$ python3.6 -m venv --without-pip virtual`
`$ source virtual/bin/activate`
then run this command to install pip addons`$ curl https://bootstrap.pypa.io/get-pip.py | python`

- Run the following in the start.sh file to prepare your internet environment to run.
```zsh or bash
$ export DATABASE_URL='postgresql+psycopg2://your username:your password@localhost/pitch'
$ export SECRET_KEY='Your secret key'
```

- Run this commands to be able to migrate your database to application.
```zsh or bash 
$ python manage.py db init
$ python manage.py db migrate -m "initial migration"
$ python manage.py db upgrade
```
- In the same terminal type use this command to run your application:
`$ python3 manage.py server` then open the browser at `http://localhost:5000/`

## Known bugs

SQLAlchemy errors, automatic sign out has a short time span

## Technologies used

    - Python 3.6
    - HTML
    - Bootstrap 4
    - JavaScript
    - Heroku
    - Postgresql

### Contact details

You can contact me at danmark.chemuren@gmail.com for any feedback.

### License

This is a [MIT licensed](/LICENSE) application.

Copyright (c) **Danmark Mutai**
