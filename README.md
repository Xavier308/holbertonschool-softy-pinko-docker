# Docker Project

This project demonstrates the containerization of a web application using Docker, with separate containers for the front-end, back-end, and a proxy server.

## Key Terms

- **Docker**: A platform for developing, shipping, and running applications in containers.
- **Nginx**: A web server that can also be used as a reverse proxy, load balancer, and HTTP cache.
- **Server**: A computer program or device that provides functionality for other programs or devices, called clients.
- **Proxy**: An intermediary server that forwards requests from clients to other servers.
- **Load Balancer**: A device that distributes network or application traffic across multiple servers.

## Important Commands

### Building Docker Images

```bash
docker build -f ./Dockerfile -t softy-pinko:task0 .
```

### Running Docker Containers

```bash
docker run -p 5252:5252 -it --rm --name softy-pinko-task1 softy-pinko:task1
```

### Using Docker Compose

Build services:
```bash
docker-compose build
```

Start services:
```bash
docker-compose up
```

Scale services:
```bash
docker-compose up --scale back-end=2
```
Front-end
```bash
http://localhost:9000

http://localhost
```
## Project Structure

1. **Task 0**: Create your first Docker image
2. **Task 1**: Set up the back-end
3. **Task 2**: Set up the front-end
4. **Task 3**: Connect the front-end and back-end
5. **Task 4**: Implement Docker Compose
6. **Task 5**: Add a proxy server
7. **Task 6**: Scale horizontally

## Technologies Used

- Docker
- Docker Compose
- Nginx
- Flask
- Python
