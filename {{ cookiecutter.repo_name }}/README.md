# {{cookiecutter.project_name}}

## PostgreSQL
**postgres password**: {{cookiecutter.postgres_password}}

**database url**: postgres://{{cookiecutter.postgres_user}}:{{cookiecutter.postgres_password}}@postgres/{{cookiecutter.postgres_user}}?sslmode=disable

## Hosts
**Web**: {{cookiecutter.virtual_host}}

**Pgweb**: pgweb.{{cookiecutter.virtual_host}}

## Commands

Run Django manage.py commands:

    docker-compose run --rm web ./manage.py help
    docker-compose run --rm web ./manage.py migrate
    docker-compose run --rm web ./manage.py createsuperuser
    docker-compose run --rm web ./manage.py collectstatic
    docker-compose run --rm web ./manage.py startapp APP_NAME
