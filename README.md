# Team project: api_yamdb - service that collects user feedback on movies, books etc.

## Project description:

The YaMDb project collects users' feedbacks and ratings on movies, books etc.

Items are divided into categories such as "Books", "Films", "Music". The list of categories can be expanded (for example, you can add the category "fine art" or "jewellery").
Categories are devideded into genres from the predefined list (for example, Fairy Tale, Rock or Arthouse).
Only the administrator can add new categories and genres.

Users may add reviews and ratings.
From user ratings, an average rating is formed.
User can leave only one review per item.

Only authenticated users can add reviews, comments and ratings.

The project is accessed via API.

## How to launch a project:

Clone the repository and switch to it on the command line:
```
git clone git@github.com:Artem-Ter/api_yamdb.git
or
git clone https://github.com/Artem-Ter/api_yamdb.git

```
```
cd api_yamdb
```
Create and activate virtual environment:
```
python3 -m venv env
```
```
source env/bin/activate
```
```
python3 -m pip install --upgrade pip
```

Install dependencies from a file requirements.txt:
```
pip install -r requirements.txt
```

Create .env file, see example below:
```
    #Turn on DB Postgres or SQLite
    POSTGRES_ON=True
    #Parameters to connect DB Postgres
    DB_NAME=postgres_db
    POSTGRES_USER=postgres_user
    POSTGRES_PASSWORD=SuperStrongPassword
    DB_HOST=127.0.0.1
    DB_PORT=5432
```

Make migrations:
```
python3 manage.py makemigrations
```
```
python3 manage.py migrate
```

Run project:
```
python3 manage.py runserver 8000
```

## Endpoints description and detailed API documentation is availalbe at:
```
http://127.0.0.1:8000/redoc/
```

## Technologies used:

- Python;
- Django Framework;
- Django-Rest-Framework;
- JWT.

## Project author
[Artem Tereschenko](https://github.com/Artem-Ter)
