# DOCKER DESCRIPTION & USEFUL COMMANDS IN DETAIL

Docker is a platform for developing, shipping, and running applications in containers. 
Containers are lightweight, portable, and self-sufficient units that can run 
applications and their dependencies in isolated environments. Docker provides a 
consistent and reproducible environment across different machines, making it easier 
to manage and deploy applications.

<b>Here are the key components of Docker:</b>

1. <B>Docker Engine:</B> The core of Docker is the Docker Engine, which is responsible 
for building, running, and managing containers. It consists of a server 
(daemon) and a REST API that allows you to interact with the daemon.

2. <b>Docker Images:</b> Images are lightweight, standalone, and executable packages 
that include everything needed to run a piece of software, including the code, 
runtime, libraries, and system tools. Images are used to create containers.

3. <b>Docker Containers:</b> Containers are instances of Docker images that run in 
isolated environments. They encapsulate an application and its dependencies, 
ensuring consistency across different environments. Containers are portable 
and can run on any system that supports Docker.

<b>Some of the commonly used docker commands.</b> 

• <b>docker images</b>: List all Docker images on your local machine.<br>
• <b> docker pull <image_name>:</b> Download a Docker image from a registry.  <br>
• <b> docker rmi <image_name>:</b> Remove a Docker image from your local machine. <br> 
• <b> docker ps:</b> List running containers.  <br>
• <b> docker ps -a:</b> List all containers (running and stopped).  <br>
• <b> docker run <options> <image_name>:</b> Create and start a container based on a Docker image.  <br>
• <b> docker start <container_id or container_name>:</b> Start a stopped container.  <br>
• <b> docker stop <container_id or container_name>:</b> Stop a running container.  <br>
• <b> docker restart <container_id or container_name>:</b> Restart a running or stopped container.  <br>
• <b> docker rm <container_id or container_name>:</b> Remove a stopped container.  <br>
• <b> docker inspect <container_id or container_name>:</b> Display detailed information about a container.  <br>
• <b> docker logs <container_id or container_name>:</b> View the logs of a container.  <br>
• <b>  docker exec -it <container_id or container_name> <command>:</b> Execute a command in a running container interactively.  <br>
• <b> docker run -it <image_name> /bin/bash:</b> Run a container and enter into its shell interactively.  <br>
• <b> docker-compose up:</b> Create and start containers defined in a docker-compose.yml file.  <br>
• <b> docker-compose down:</b> Stop and remove containers created by docker-compose up.  <br>
• <b> docker-compose ps:</b> List containers managed by Docker Compose.  <br>
• <b>  docker login:</b> Log in to a Docker registry.  <br>
• <b> docker push <image_name>:</b> Push a Docker image to a registry.  <br>
• <b>  docker tag <image_name> <new_image_name>:</b> Tag a Docker image.  <br>
• <b>  docker logout:</b> Log out from a Docker registry.  <br>
• <b> docker network ls:</b> List Docker networks.  <br>
• <b> docker network inspect <network_id or network_name>:</b> Display detailed information about a Docker network. <br>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
<b>DOCKER CONCEPT WITH BASED ON COMMANDS </b> <br>

 𝗜𝗺𝗮𝗴𝗲 𝗠𝗮𝗻𝗮𝗴𝗲𝗺𝗲𝗻𝘁
- Use 𝚍𝚘𝚌𝚔𝚎𝚛 𝚋𝚞𝚒𝚕𝚍 to create images from Dockerfiles, the blueprint for containers.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚙𝚞𝚕𝚕 to download pre-built images from registries like Docker Hub.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚙𝚞𝚜𝚑 to upload your images to remote registries.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚒𝚖𝚊𝚐𝚎𝚜 lists locally stored images. 
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚛𝚖𝚒 removes unwanted images.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚝𝚊𝚐 tags images for organizational purposes.

🟡 𝗖𝗼𝗻𝘁𝗮𝗶𝗻𝗲𝗿 𝗟𝗶𝗳𝗲𝗰𝘆𝗰𝗹𝗲 
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚛𝚞𝚗 launches a container from an image.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚜𝚝𝚘𝚙 and 𝚍𝚘𝚌𝚔𝚎𝚛 𝚔𝚒𝚕𝚕 halt running containers gracefully or forcibly.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚛𝚎𝚜𝚝𝚊𝚛𝚝 restarts a stopped container.  
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚛𝚎𝚗𝚊𝚖𝚎 to rename existing containers.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚕𝚘𝚐𝚜 prints logs of a container.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚎𝚡𝚎𝚌 runs commands interactively in a container.

🟡 𝗡𝗲𝘁𝘄𝗼𝗿𝗸𝗶𝗻𝗴 𝗮𝗻𝗱 𝗦𝘁𝗼𝗿𝗮𝗴𝗲
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚗𝚎𝚝𝚠𝚘𝚛𝚔 manages custom networks containers connect to.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚟𝚘𝚕𝚞𝚖𝚎 creates sharable storage volumes containers can mount.

🟡 𝗠𝗮𝗶𝗻𝘁𝗲𝗻𝗮𝗻𝗰𝗲
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚜𝚢𝚜𝚝𝚎𝚖 𝚙𝚛𝚞𝚗𝚎 cleans up unused containers, images, volumes, etc.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚛𝚖 deletes stopped containers.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚒𝚗𝚜𝚙𝚎𝚌𝚝 shows in-depth info on a container.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚜𝚝𝚊𝚝𝚜 provides real-time container resource usage stats.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚙𝚜 lists running containers.

🟡 𝗗𝗼𝗰𝗸𝗲𝗿 𝗖𝗼𝗺𝗽𝗼𝘀𝗲 
- 𝚍𝚘𝚌𝚔𝚎𝚛-𝚌𝚘𝚖𝚙𝚘𝚜𝚎 𝚞𝚙 starts an multi-container app from a compose file.
- 𝚍𝚘𝚌𝚔𝚎𝚛-𝚌𝚘𝚖𝚙𝚘𝚜𝚎 𝚍𝚘𝚠𝚗 stops and destroys the resources.
- 𝚍𝚘𝚌𝚔𝚎𝚛-𝚌𝚘𝚖𝚙𝚘𝚜𝚎 𝚕𝚘𝚐𝚜 aggregates logs from the containers.

🟡 𝗔𝗱𝗱𝗶𝘁𝗶𝗼𝗻𝗮𝗹 𝗖𝗼𝗺𝗺𝗮𝗻𝗱𝘀
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚌𝚙 copies files between host and containers.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚍𝚒𝚏𝚏 shows filesystem changes in a container.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚝𝚘𝚙 displays running processes in a container.
- 𝚍𝚘𝚌𝚔𝚎𝚛 𝚜𝚎𝚊𝚛𝚌𝚑 searches for images on Docker Hub.
