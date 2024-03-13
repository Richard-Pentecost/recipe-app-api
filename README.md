# recipe-app-api

Recipe API project

# docker commands

command for running tests inside docker: docker-compose run --rm app sh -c "python manage.py test"
command for making migrations inside docker: docker-compose run --rm app sh -c "python manage.py makemigrations"
command for running migrations inside docker: docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

list volumes: docker volumes ls
remove volumes: docker volume rm "volume name"

create a super user: docker-compose run --rm app sh -c "python manage.py createsuperuser"
