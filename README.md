# twitoff- 16


## Installation

Download the repo and navigate there from the command line:

```sh
git clone git@github.com:Malven2019/twitoff.git
cd twitoff
```

## Setup

Setup and activate the virtual environment:
```sh
pipenv install
pipenv shell
```
Setup the database:

```sh
# Windows users can omit the "FLASK_APP=web_app" partF...

FLASK_APP=web_app flask db init #> generates app/migrations dir

# run both when changing the schema:
FLASK_APP=web_app flask db migrate #> creates the db (with alembic_version" table)
FLASK_APP=web_app flask db upgrade #> creates the specified tables
```

## Usage

Run the web app:

    ``` sh
    FLASK_APP = web_app flask run
    ```
