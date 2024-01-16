# DOCKER

>  Docker is a tool for creating and managing a container.

# IMAGES
> Images are blueprints for containers. They are read-only and contain the application as well as the necessary application environment.
Images do not run themselves, instead they can be executed as containers.

# CONTAINER
> Containers are running instances of images. When you create a container a
thin read-write layer is added on top of the Image.

### SOME USEFUL DOCKER COMMANDS:


```
< image_name > : name of the image
< container_name > : name of the container
< image_id > : id of the image
```

|  | Use | Commands
| :-------- | :-------------- | :--------------- | 
| 1. | to build an image | docker build .
| 2. | to build an image with name | docker build -t [any name to the image]:[version] .
| 3. | to list all the images | docker images
| 4. | to create and start a container | docker run <image_name>
| 5. | to create a container with name| docker run --name [any name to the container]
| 6. | to publish the port for your container | docker run -p [host_port]:[container_port] <image_name>
| 7. | to list all the running container | docker ps
| 8. | to list all the container including the stopped container | docker ps -a
| 9.  | run the container in interactive mode | docker run -it <image_name>
| 10. | to start a container. **Note: it would run the container in detached mode** | docker start <conatiner_name>
| 11. | to stop a container | docker stop <container_name>
| 12. | to run the container in detached mode | docker run -d <image_name>
| 13. | to see the logs at the time of execution | docker logs <container_name>
| 14. | to follow logs output | docker logs -f <container_name>
| 15. | if you want the container in attach mode | docker attach <container_name>
| 16. | to start a container in attach mode | docker start -a <container_name>
| 17. | to remove the image | docker rmi <image_name>
| 18. | to remove the container | docker rm <container_name>
| 19. | to remove all the images | docker images prune
| 20. | to remove the container automatically when stopped | docker run --rm <image_id>
| 21. | to display detailed information of image | docker image inspect <image_id>
| 22. | to copy any directory from local machine to container  | docker cp <local_path> <conatainer_name>:<oath inside the container> **docker cp dummy/. vat:/tests**
| 23. | to copy any directory from container to local machine  | docker cp <conatainer_name>:<path inside the container> <local_path> 
| 24. | to remove all the images | docker images prune
| 25. | to push the image to docker registory | docker push <image_name>
| 26. | to pull the image from the regsitory | docker pull <image_name>
| 27. | to rename an image | docker tag <old_name> <new_name>
| 28. | to save the image in your local computer as tar file| docker save --output image.tar <image_name>
| 29. | to login to the docker registory | docker login
| 30. | to logout from the docker registory | docker logout
