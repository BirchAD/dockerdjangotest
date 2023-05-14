# Django API Project

This is a Django API application built using Test-Driven Development (TDD) methodology. The application is containerized using Docker and is continuously integrated using GitHub Actions. The API is documented using Swagger.

## Requirements

- Python 3.8+
- Django 3.2+
- Docker
- docker-compose

## Getting Started

### With Docker

1. Clone the repository:
```bash
git clone https://github.com/username/repo.git](https://github.com/BirchAD/dockerdjangotest/
cd dockerdjangotest
```

2. Build the Docker image:
```bash
docker-compose build
```

3. Start the Docker container:
```bash
docker-compose up
```
The application should be running at `http://localhost:8000`.

### Locally without Docker

1. Clone the repository:
```bash
git clone https://github.com/username/repo.git](https://github.com/BirchAD/dockerdjangotest/
cd dockerdjangotest
```

2. Install dependencies:
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
The application should be running at `http://localhost:8000`.

## Running Tests

To run tests, use the following command:

```bash
docker-compose run app sh -c "python manage.py test && flake8"
```

If running tests locally:

```bash
python manage.py test && flake8
```

## GitHub Actions

The application uses GitHub Actions for Continuous Integration. On every push to the main branch, the action will run the tests and check code style using flake8.

## API Documentation

You can view the API documentation at `http://localhost:8000/swagger`. The documentation is built using Swagger.
https://choosealicense.com/licenses/mit/)
