Reload terminal `source ~/.zshrc`

[Setting up SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

`build docker .`  
The docker build command builds Docker images from a Dockerfile and a “context”. A build’s context is the set of files located in the specified PATH or URL. The build process can refer to any of the files in the context. For example, your build can use a COPY instruction to reference a file in the context.

`docker-compose run --rm app sh -c "flake8"` 
Runs flake8

`docker-compose run --rm app sh -c "django-admin startproject app ."`
Creats Django project in workspace

`docker-compose up`
runs docker services

Browser src = http://127.0.0.1:8000/

`docker-compose run --rm app sh -c "python manage.py test"`
runs Django test

`docker-compose run --rm app sh -c "python manage.py startapp [NAME OF APP] "`
Django command for starting a new app

`docker-compose run --rm app sh -c "python manage.py
 wait_for_db && python manage.py migrate"`
 run backend

`docker-compose down` to turn off db then ` docker volume rm recipe-app-api_dev-db-data
recipe-app-api_dev-db-data` to remove user from docker then `docker volume ls` to check is user has been removed

`code .zshrc`
`alias docker-python-test='docker-compose run --rm app sh -c "python manage.py test"'`
`alias reload="source ~/.zshrc"`
to add custom commands for terminal
