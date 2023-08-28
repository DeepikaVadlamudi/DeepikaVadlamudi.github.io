![container](/assets/images/Container.png)
<p>Docker has brought about a significant transformation in the realm of software development and deployment by introducing a streamlined and effective method for encapsulating applications within containers. Docker simplifies the process of building, delivering, and executing applications across various environments. In order to assist you in navigating the Docker landscape more proficiently, I have curated a comprehensive reference guide containing fundamental commands and key principles. So, let’s delve into it without further ado!</p>

### Docker Basics 

<p>Images: Docker images serve as the foundation for containers. They are read-only templates that contain everything needed to run a specific application, including the code, runtime, libraries, and dependencies.</p>

<p>Containers: Containers are the instances of Docker images. They are isolated and lightweight, providing a consistent and reproducible environment for running applications. Containers can be started, stopped, and deleted as needed.</p>

<p>Dockerfile: A Dockerfile is a text file that contains instructions for building a Docker image. It specifies the base image, adds necessary dependencies, copies files, and configures the container environment.</p>

<p>Registry: Docker registries are repositories that store Docker images. The default public registry is Docker Hub, which hosts a vast collection of pre-built images. However, you can also utilize private registries for secure image storage.</p>

<p>Volumes: Docker volumes are used to persist data and share files between containers and the host system. They allow data to be stored independently of the container lifecycle, ensuring data integrity and persistence.</p>

<p>Networking: Docker enables the creation of networks to connect containers together. Networks facilitate communication between containers, allowing them to interact and share resources.
</p>

### Installing docker

<p>There are two methods for installing Docker on Mac:
</p>

1. One approach involves installing VirtualBox, setting up a Linux virtual machine, and then installing Docker within that virtual machine.
2. The alternative method is to directly install the Docker application on your Mac.

### Docker Commands
1. Build and Run:
   * `docker build -t image_name .`: Builds an image using the Dockerfile located in the current directory.
   * `docker run image_name`: Runs a container based on a specific image.
   * `docker run -it image_name`: Runs a container interactively, providing a terminal for interaction.
   * `docker run -p host_port:container_port image_name`: Maps a container port to a port on the host system, enabling external access.
   * `docker run -v host_path:container_path image_name`: Mounts a host directory or file as a volume within the container.
2. Managing containers:
   * `docker ps`: Lists the running containers.
   * `docker ps -a`: Lists all containers, including the stopped ones.
   * `docker start container_id/container_name`: Starts a stopped container.
   * `docker stop container_id/container_name`: Stops a running container gracefully.
   * `docker rm container_id/container_name`: Removes a container.
   * `docker logs container_id/container_name`: Displays the logs of a container.
3. Managing Images:
  * `docker images`: Lists all available images.
  * `docker pull image_name`: Downloads an image from a registry.
  * `docker push image_name`: Pushes an image to a registry.
  * `docker rmi image_id/image_name`: Removes an image from the local system.
  * `docker tag source_image:tag target_image:tag`: Tags an image with a different name or version.
4. Working with Volumes:
  * `docker volume create volume_name`: Creates a Docker volume.
  * `docker volume ls`: Lists all Docker volumes.
  * `docker volume rm volume_name`: Removes a Docker volume.
  * `docker run -v volume_name:container_path image_name`: Mounts a Docker volume in a container.
5. Networking:
  * `docker network create network_name`: Creates a Docker network.
  * `docker network ls`: Lists all Docker networks.
  * `docker network rm network_name`: Removes a Docker network.
  * `docker run --network=network_name image_name`: Runs a container within a specific network.

<p>This cheat sheet provides a solid foundation for working with Docker. By familiarizing yourself with these commands and concepts, you can effectively build, manage, and deploy applications using Docker containers. As you delve further into the Docker ecosystem, explore the extensive Docker documentation for more advanced features and possibilities.</p>

<p>Happy Docking!</p>


