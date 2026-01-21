# Docker-Node

A simple Node.js application containerized with Docker for practicing Docker concepts.

## Description

This project demonstrates how to containerize a basic Express.js server using Docker. The application runs on port 8000 and responds with a JSON message: "Hello, World! this side docker".

## Prerequisites

- Docker installed on your system
- Node.js (optional, for local development)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/pbbhattpriyanshu/Docker-Node.git
   cd Docker-Node
   ```

2. Build the Docker image:
   ```bash
   docker build -t docker-node .
   ```

## Usage

1. Run the container:
   ```bash
   docker run -p 8000:8000 docker-node
   ```

2. Open your browser and navigate to `http://localhost:8000` to see the response.

## Local Development

If you want to run the application locally without Docker:

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the server:
   ```bash
   node main.js
   ```

The server will run on `http://localhost:8000`.

## Project Structure

- `Dockerfile`: Docker configuration for building the image
- `main.js`: Main Express.js application file
- `package.json`: Node.js dependencies and scripts
- `package-lock.json`: Lockfile for dependencies

## License

ISC
