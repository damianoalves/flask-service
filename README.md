# Flask API

This is a Flask API that I will keep improving with new features and functionalities.
This boilerplate can be used as a template for bigger projects.


### Introduction

The “micro” in microframework means Flask aims to keep the core simple but extensible. Flask won’t make many decisions for you, such as what database to use.

By convention, templates and static files are stored in subdirectories within the application’s Python source tree, with the names templates and static respectively.

### Dependencies

* [Python](https://www.python.org/) - Programming Language
* [Flask](https://flask.palletsprojects.com/) - The framework used
* [SQLAlchemy](https://docs.sqlalchemy.org/) - ORM
* [Pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
* [Alembic](https://alembic.sqlalchemy.org/) - Database Migrations
* [Pipenv](https://pypi.org/project/pipenv/) - Dependency Management

### Development Dependencies
* [Flake8](https://flake8.pycqa.org/en/latest/) - Code Linting
* [Black](https://black.readthedocs.io/en/stable/) - Code Formatter
* [Isort](https://pycqa.github.io/isort/) - Import Sorter
* [Mypy](https://mypy.readthedocs.io/en/stable/) - Static Type Checker
* [Pylama](https://pylama.readthedocs.io/en/latest/) - Code Linting
* [Pre-commit](https://pre-commit.com/) - Git Hooks
* [Yamllint](https://yamllint.readthedocs.io/en/stable/) - YAML Linter

### Virtual environments

```
$ pip install pipenv
$ pipenv shell
```

Install all project dependencies using:

```
$ pipenv install
```

Install all development dependencies using:

```
$ pipenv install --dev
```

Install pre-commit hooks:

```
$ pre-commit install
```

### Running
 
```
$ flask run
```

This launches a very simple builtin server, which is good enough for testing but probably not what you want to use in production.

If you enable debug support the server will reload itself on code changes, and it will also provide you with a helpful debugger if things go wrong.

If you have the debugger disabled or trust the users on your network, you can make the server publicly available simply by adding --host=0.0.0.0 to the command line:

```
flask run --host=0.0.0.0
```

### Running using Manager

This app can be started using Flask Manager. It provides some useful commands and configurations, also, it can be customized with more functionalities.

```
python manage.py runserver
```

### Alembic Migrations

Use the following commands to create a new migration file and update the database with the last migrations version:

```
flask db revision --autogenerate -m "description here"
flask db upgrade head
```

This project also uses the customized manager command to perform migrations.
```
python manage.py db revision --autogenerate -m "description here"
python manage.py db upgrade head
```

To upgrade the database with the newest migrations version, use:

```
python manage.py db upgrade head
```

For more information, access [Auto generating migrations](https://alembic.sqlalchemy.org/en/latest/autogenerate.html).


## Contributing

This API was developed based on:

[Flask documentation](https://flask.palletsprojects.com/)

[SQLAlchemy documentation](https://docs.sqlalchemy.org/)

[Pydantic documentation](https://pydantic-docs.helpmanual.io/)

[Alembic documentation](https://alembic.sqlalchemy.org/)



## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
