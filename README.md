What is this project?

Docker-PostgreSQL is a sample of tutorial Course to start a django project with postgresql as database running on docker.

challenges that i deal with:

1-How to use Docker 2-How use PostgreSQL in this project

How to use?

If you want to get notified about the future changes Follow my github account.

First clone the project.

If you are on windows click on the Docker Desktop icon and wait for about a minute. Then in the project directory run this command:

docker-compose up --build It will create two containers: One for Django and one for PostgreSql as the database for the project. All the required packages will be installed.

Install a new package. Attention: If you want to install a package for django project you should run this command: docker-compose exec web pip install

Don't forget to add the new package to requirements.txt for further use:

docker-compose exec web pip freeze > requirements.txt
