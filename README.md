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

`git clone https://github.com/laravel-geek/laravel-livewire-docker.git`

2. Navigate to the project directory:

`cd laravel-livewire-docker`


3. Launch the Docker containers:

`docker-compose up nginx -d`


### Configuration

- To access the Laravel application, go to http://localhost in your web browser.
- To execute Artisan commands, use:

`docker-compose run --rm artisan <command>`

- To work with Composer:

`docker-compose run --rm composer <command>`


## Project Structure

Description of the file structure and main configuration settings.

- `docker-compose.yml` - Main Docker Compose file.
- `./docker/nginx` - Configuration for the Nginx server.
- `./docker/php` - Dockerfile and configurations for the PHP container.
- `./docker/postgres` - Configurations for the PostgreSQL container.
- `./docker/composer` - Dockerfile for Composer.

## Using This Repository to Launch a New Laravel Project

To use this setup as a foundation for deploying a new Laravel project, follow these steps:

1. **Create a new GitHub repository** for your new Laravel project. This allows for version control and collaboration on the project.

2. **Locally clone this Docker setup repository** (if not already done):
   `git clone https://github.com/laravel-geek/laravel-livewire-docker.git <your_new_project_name>
   cd <your_new_project_name>`
   Replace `<your_new_project_name>` with the name of your new project.

3. **Remove the existing .git history** and start a fresh history for the new project:
   `rm -rf .git
   git init
   git remote add origin <URL of your new GitHub repository>`
    Replace `<URL of your new GitHub repository>` with the URL of your new repository.

4. **Add your Laravel project source code** to the `laravel` directory. If starting a new project, you can install Laravel using Composer by running:
   `docker-compose run --rm composer create-project --prefer-dist laravel/laravel .`
   Ensure you are in the root directory of your Docker project.

5. **Configure your Laravel environment** (e.g., `.env` files) to match your Docker containers and database settings.

6. **Add, commit, and push your project to GitHub**:
   `git add .
   git commit -m "Initial commit with Docker setup for Laravel Livewire project"
   git push -u origin main`

## Contributing

Contributions to the development of the project are welcome. If you wish to contribute, please first discuss the changes you wish to make via an issue.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

If you have any questions or suggestions, please feel free to reach me out.