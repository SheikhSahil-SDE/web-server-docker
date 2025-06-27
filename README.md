# Web Server with Docker

This project is a simple web server built using Node.js and Docker. It demonstrates how to set up a web server, define routes, and handle requests, all while utilizing Docker for containerization.

## Project Structure

```
web-server-docker
├── src
│   ├── app.js         # Main application logic
│   └── index.js       # Entry point for the application
├── Dockerfile          # Instructions for building the Docker image
├── docker-compose.yml  # Defines services and configurations for Docker
├── .dockerignore       # Files to ignore when building the Docker image
├── package.json        # npm configuration file
└── README.md           # Project documentation
```

## Getting Started

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed on your machine
- [Docker Compose](https://docs.docker.com/compose/install/) installed

## Building the Docker Image

To build the Docker image for the web server, run the following command in the project root directory:

```
docker build -t web-server-docker .
```

## Running the Application

To run the web server using Docker Compose, execute:

```
docker-compose up
```

This command will start the web server and any other defined services.

## Accessing the Web Server

Once the server is running, you can access it at [http://localhost:3000](http://localhost:3000) (or the port specified in your configuration, e.g., in `docker-compose.yml`).

## Stopping the Application

To stop the running application, use:

```
docker-compose down
```

## License

- This project is licensed under the MIT License. See the LICENSE file for details.
