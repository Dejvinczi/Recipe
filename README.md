# Recipe

This project is a Recipe Manager built with Django and Django REST Framework. It allows users to create, view, update, and delete recipes through a REST API.
## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Usage](#usage)
## Features
- **User registration**: API for creating new system users for authentication purposes. 
- **Recipes management**: Authorised users of the system can manage (view, create, edit, delete) recipes. . 
- **Ingredients management**: Authorised users of the system can manage (view, edit, delete) recipe ingredients. 
- **Tags management**: Authorised users of the system can manage (view, edit, delete) recipe tags. 

## Requirements

- **Python**: This application requires **Python 3.9** or later. You can download and install Python from the [official Python website](https://www.python.org/).

- **Docker**: Ensure that Docker is installed on your system. You can download and install Docker Desktop from the [official Docker website](https://www.docker.com/).

- **Docker Compose**: Docker Compose is used for orchestrating multi-container Docker applications. It should be included with Docker Desktop installation on most platforms. If not, make sure to install Docker Compose separately following the instructions provided on the [Docker Compose documentation](https://docs.docker.com/compose/install/).

## Getting Started

### Installation

1. **Clone the repository**: Clone the repository to your local machine using Git:
    ```bash
    git clone https://github.com/Dejvinczi/Recipe.git
    ```

2. **Create .env**: Create an .env file from the .env.sample:
    ```bash
    cp .env.sample .env
    ```

4. **Set Up Environment Variables**: 
    ```bash
    DB_NAME=dbname
    DB_USER=rootuser
    DB_PASS=changeme
    DJANGO_SECRET_KEY=changeme
    DJANGO_ALLOWED_HOSTS=127.0.0.1
    ```

5. **Build Docker containers**: Use Docker Compose to build the Docker containers defined in the composition file `docker-compose.yaml`:
    ```bash
    docker-compose build
    ```

### Usage
- **Start Docker containers**: Start the Docker containers using Docker Compose:
    ```bash
    docker-compose up
    ```
