# Recipe-API

A REST API with Python and Django built in a Test Driven Development

## Supported Functionality

- User Authentication
- Creating Objects
- Filtering and Sorting Objects
- Uploading and Viewing Images

## Features:

- 19 API Endpoints - Managing users, recipes, tags, ingredients
- User Authentication
- Browseable Admin Interface (Django Admin)
- Browsable API (Swagger)

## Technologies:

- Python
- Django
- Django REST framework
- Postgres
- Docker
- Swagger
- Github Actions
- AWS

## Django Project Structure

- app/ - Django project
- app/core/ - Code shared between multiple apps
- app/user/ - User related code
- app/recipe/ - Recipte related code

## Why use Docker?

- Consistent dev and prod environment
- Easier collaboration
- Capture all dependencies as code
- Easier cleanup

## Configure Docker

- Create a Dockerfile
- Lists steps for creating image
  - Choose a base image (python)
  - Install dependencies
  - Setup users

# Docker Compose

- How our Docker image(s) should be used
- Define our "services"
  - Name (eg:app)
  - Port mappings
  - Volume mappings

# Using Docker Compose

- Run all commands through Docker Compose
  > > docker-compose run --rm app sh -c "python manage.py collectstatic"
- docker-compose runs a Docker Compose commands
- run will start a specific container defined in config
- --rm removes the container
- app is the name of the service
- sh -c passes in a shell command
- Command to run inside container

# What is Linting?

- Tool to check code formatting
- Highlight errors, typos, formatting issues
