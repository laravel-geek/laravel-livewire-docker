# Laravel Livewire Docker Setup

This project provides a Docker setup for developing Laravel applications with Livewire. It simplifies the process of setting up and running a development environment for Laravel projects.

## Features

- Complete Docker setup for a development environment.
- Supports Laravel and Livewire.
- Incorporates configurations for Nginx, PHP, and PostgreSQL, alongside utility containers for Composer and Artisan services.

## Getting Started

To get started with this project, ensure you have Docker and Docker Compose installed on your system.

### Installation

1. Clone the repository to your local machine:

git clone https://github.com/laravel-geek/laravel-livewire-docker.git

2. Navigate to the project directory:

cd laravel-livewire-docker


3. Launch the Docker containers:

docker-compose up nginx -d


### Configuration

- To access the Laravel application, go to http://localhost in your web browser.
- To execute Artisan commands, use:

docker-compose run --rm artisan <command>

- To work with Composer:

docker-compose run --rm composer <command>


## Project Structure

Description of the file structure and main configuration settings.

- `docker-compose.yml` - Main Docker Compose file.
- `./docker/nginx` - Configuration for the Nginx server.
- `./docker/php` - Dockerfile and configurations for the PHP container.
- `./docker/postgres` - Configurations for the PostgreSQL container.
- `./docker/composer` - Dockerfile for Composer.

## Contributing

Contributions to the development of the project are welcome. If you wish to contribute, please first discuss the changes you wish to make via an issue.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

If you have any questions or suggestions, please feel free to reach me out.