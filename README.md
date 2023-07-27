# Django API Project: REST API with Django, Docker, and Test-Driven Development

Welcome to my project! This is an advanced REST API built using Python, Django (3.2), Django REST Framework (3.12), Docker, GitHub Actions, and Postgres, following the principles of Test-Driven Development. 

This API forms the backend of a recipe app, where you can store, view, and manage some of your favorite recipes.

## Project Features

- **User Authentication:** Handle user registration, login, and management of user profiles.
- **Creating Objects:** Ability to create recipe objects with attributes like title, ingredients, cooking time, and price.
- **Filtering and Sorting Objects:** Functionality to search for recipes based on different criteria, and sort the results.
- **Uploading and Viewing Images:** Capability to upload images to each recipe.
- **Docker and Docker-Compose:** The project is fully containerized using Docker for easy replication and deployment.
- **Continuous Integration with GitHub Actions:** The project is setup with GitHub Actions for Continuous Integration, automatically running linting and unit tests.
- **Test-Driven Development:** The project follows the principles of Test-Driven Development, with comprehensive test coverage.
- **Postgres Database:** The backend database used is Postgres, professionally configured for this project.

## Prerequisites

You'll need the following installed to run the project:
- Python 3.8+
- Django 3.2+
- Docker
- docker-compose

## Getting Started

### With Docker
1. Clone the repository:
```bash
git clone https://github.com/username/repo.git
cd repo
```
2. Build the Docker image:
```bash
docker-compose build
```
3. Start the Docker container:
```bash
docker-compose up
```
The application should now be running at `http://localhost:8000`.

### Without Docker
1. Clone the repository:
```bash
git clone https://github.com/username/repo.git
cd repo
```
2. Install the dependencies:
```bash
pip install -r requirements.txt
```
3. Run migrations:
```bash
python manage.py migrate
```
4. Start the server:
```bash
python manage.py runserver
```
The application should now be running at `http://localhost:8000`.

## Running Tests
To run the tests with Docker, use the following command:
```bash
docker-compose run app sh -c "python manage.py test && flake8"
```
To run the tests without Docker, use:
```bash
python manage.py test && flake8
```

## GitHub Actions

The application uses GitHub Actions for Continuous Integration. On every push to the main branch, the action will run the tests and check code style using flake8.

## API Documentation

You can view the API documentation at `http://localhost:8000/swagger`. The documentation is built using Swagger.
https://choosealicense.com/licenses/mit/)
