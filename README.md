
# Frappe Docker

This repository contains a Dockerized setup for running the [Frappe framework](https://frappeframework.com/). It simplifies the deployment and management of Frappe applications by leveraging Docker containers for scalability and ease of use.

## Features

- Pre-configured Docker environment for Frappe.
- Scalable architecture with Docker Compose.
- Easy setup for local development and production.
- Customizable for different versions of Frappe and ERPNext.
- Includes configurations for databases, caching, and queue workers.

## Prerequisites

Before setting up the project, ensure you have the following installed:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/Mostafa-Rawash/frappe-docker.git
   cd frappe-docker
   ```

2. Copy the `.env.example` file to `.env` and configure it based on your requirements:

   ```bash
   cp .env.example .env
   ```

3. Build and start the containers:

   ```bash
   docker-compose up -d
   ```

4. Access the Frappe instance in your browser:

   ```
   http://localhost:8000
   ```

   Replace `8000` with your configured port if changed.

## Configuration

- **Database**: Configure the database settings in the `docker-compose.yml` file or `.env` file.
- **Environment Variables**: Modify `.env` to customize your setup.
- **Volumes**: Persistent storage is set up via Docker volumes for data and logs.

## Usage

- **Start the environment**:

  ```bash
  docker-compose up -d
  ```

- **Stop the environment**:

  ```bash
  docker-compose down
  ```

- **Logs**:

  ```bash
  docker-compose logs -f
  ```

- **Enter a container**:

  ```bash
  docker exec -it <container_name> bash
  ```

## Contributing

Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.

1. Fork the repository.
2. Create your feature branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add some feature"
   ```

4. Push to the branch:

   ```bash
   git push origin feature/your-feature-name
   ```

5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For any questions or support, feel free to contact **Mostafa Rawash** via [mostafa@rawash.com](mailto:mostafa@rawash.com).
