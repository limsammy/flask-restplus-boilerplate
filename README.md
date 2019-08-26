# Boilerplate Flask REST API

Original project + README located [here](https://github.com/cosmic-byte/flask-restplus-boilerplate)

Setup
===

## Dependencies

  * pip3
  * virtualenv

## Installation

Part 1.

  1. Create new virtual env named venv: `virtualenv venv`
  2. Activate environment: `source venv/bin/activate`
  3. Install pip dependencies: `pip install -r requirements.txt`
  4. Update requirements: `pip freeze > requirements.txt`
  5. Setup database and configure (after creating) `.env` file with your DB keys `touch .env`
  6. At this point you should be able to start the api with `python manage.py run`

Part 2.

  1. initialize db migrations with: `python manage.py db init`
  2. generate new migration `python manage.py db migrate --message 'initial database migration'`
  3. write migration `python manage.py db upgrade`
  4. Verify all tests passing `python manage.py test`
