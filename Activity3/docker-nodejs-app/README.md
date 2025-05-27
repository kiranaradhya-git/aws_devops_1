# Docker Node.js Application

This project is a simple Node.js application that runs inside a Docker container. It sets up a basic HTTP server and listens on a specified port.

## Project Structure

```
docker-nodejs-app
├── src
│   └── index.js        # Entry point of the application
├── Dockerfile           # Dockerfile to build the image
├── .dockerignore        # Files to ignore during Docker build
├── package.json         # npm configuration file
└── README.md            # Project documentation
```

## Getting Started

To build and run the Docker container for this Node.js application, follow these steps:

1. **Clone the repository** (if applicable):
   ```bash
   git clone <repository-url>
   cd docker-nodejs-app
   ```

2. **Build the Docker image**:
   ```bash
   docker build -t docker-nodejs-app .
   ```

3. **Run the Docker container**:
   ```bash
   docker run -p 3000:3000 docker-nodejs-app
   ```

4. **Access the application**:
   Open your web browser and navigate to `http://localhost:3000`.

## Dependencies

This project uses the following dependencies:
- [http](https://nodejs.org/api/http.html) - Node.js core module for creating HTTP servers.

## License

This project is licensed under the MIT License. See the LICENSE file for details.