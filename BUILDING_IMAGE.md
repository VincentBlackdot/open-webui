# Building the TitanZ Docker Image

This guide provides steps to build and run the TitanZ Docker image locally.

## Prerequisites

- Ensure Docker is installed and running on your machine.
- Ensure Docker Compose is installed.

## Steps to Build the Image

1. **Clone the Repository**
   
   Clone the repository to your local machine if you haven't already:
   ```bash
   git clone <repository-url>
   cd open-webui
   ```

2. **Build the Docker Image**

   Use the following command to build the Docker image with the tag `titanz`:
   ```bash
   docker build -t titanz .
   ```

3. **Run the Docker Image**

   Start the container using Docker Compose:
   ```bash
   docker-compose up -d
   ```

   This command will start the services defined in the `docker-compose.yaml` file, including the `titanz` container.

4. **Access the Application**

   Once the container is running, access the application at `http://localhost:3000`.

## Additional Information

- **Logs**: Logs are stored in the `logs` directory at the root of the project.
- **Stopping Containers**: To stop the running containers, use:
  ```bash
  docker-compose down
  ```

- **Rebuilding the Image**: If you make changes and need to rebuild the image, use:
  ```bash
  docker-compose up --build -d
  ```

This documentation provides a basic overview of building and running the TitanZ Docker image. For more detailed instructions, refer to the project's main documentation or Docker's official documentation.
