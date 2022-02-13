# django-docker

## Deploying Django App inside Docker container running Apache2 with PostgreSQL, Pgadmin and Elasticsearch.

Pre-requisites:

1. Django project

2. Install Docker: https://docs.docker.com/engine/install/

3. Install Docker-compose: https://docs.docker.com/compose/install/


## Step 1: Create an empty project directory:

`mkdir project_docker && cd project_docker`

## Step 2: Create python environment:

`virtualenv env`

## Step 3: Activate an environment:
For Linux/Mac -

`source env/bin/activate`

For Windows -

`.\bin\Scripts\activate`

## Step 4: Copy the Dockerfile in your project directory.

## Step 5: Install django and psycopg2-binary library using pip:

`pip3 install django`

`pip3 install psycopg2-binary`

Freeze the requirements.txt file:

`pip3 freeze > requirements.txt`

## Step 6: Copy the file docker-compose.yml and add following content.

## Step 7: Copy the apache2 configuration file, e.g. demo_site.conf, within your root directory.

## Step 8: Deployment

For this step you need to have both docker and docker compose installed on your server or local computer.

`docker-compose up --build`

`sudo docker-compose up`

`sudo docker-compose up -d `(To run the containers in background)

`sudo docker-compose down `(To terminate the containers)
