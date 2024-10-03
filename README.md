
#`This repository contains a web application consisting of the following components:

    API: A Laravel PHP backend that serves as the API, listening on port 8000.
    Database: MySQL database service for data storage.
    Client: A Nuxt.js frontend application that interacts with the API, listening on port 3000.
    Nginx: A web server to serve the Nuxt.js application and proxy requests to the API.

project/
├── api/                        # Directory for the Laravel API
│   ├── app/                    # Laravel application logic
│   ├── artisan                 # Laravel command-line tool
│   ├── bootstrap/              # Files for bootstrapping Laravel
│   ├── config/                 # Configuration files for the application
│   ├── database/               # Database migrations and seeds
│   ├── Dockerfile              # Docker configuration for the Laravel application
│   ├── composer.json           # PHP dependencies for Laravel
│   ├── composer.lock           # Locked versions of PHP dependencies
│   ├── phpunit.xml             # PHPUnit configuration for testing
│   ├── public/                 # Publicly accessible files (e.g., index.php)
│   ├── resources/              # Views, assets, and language files for Laravel
│   ├── routes/                 # API and web routes for Laravel
│   ├── storage/                # Storage for uploaded files, logs, and caches
│   └── tests/                  # Unit and feature tests for Laravel
│
├── client/                     # Directory for the Nuxt.js client
│   ├── components/             # Reusable Vue components
│   ├── pages/                  # Pages of the Nuxt.js application
│   ├── Dockerfile              # Docker configuration for the Nuxt.js application
│   ├── nuxt.config.ts          # Nuxt.js configuration file
│   ├── package.json            # Node.js dependencies for Nuxt.js
│   ├── package-lock.json       # Locked versions of Node.js dependencies
│   ├── public/                 # Static files for the Nuxt.js app
│   └── server/                 # Server-side code for Nuxt.js (if applicable)
│   └── nginx.conf 
├── docker-compose.yml      


1.Create a Dockerfile in the api/ directory for  Laravel API:

2-Create a Dockerfile in the client/ directory for  Nuxt.js frontend
3-Create an Nginx configuration file  in the client/ directory to serve as a reverse proxy for the Nuxt.js frontend and Laravel backend

4-Create a docker-compose.yml file in the root directory to manage the services:

5-Build and Run Containers





    Build and Start Containers:
        Run docker-compose up --build to build and start all services.

    Access the Application:
        API: http://localhost:8000/api
        Client: http://localhost:3000

