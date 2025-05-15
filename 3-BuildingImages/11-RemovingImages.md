```plaintext
# Dangling Images

view all containers(including stopped)
    docker ps -a

remove all stopped containers
    docker container prune

remove all dangling images
    docker image prune

remove specific images
    docker image rm <imagename>
    docker image rm <imageID>

confirm
    docker images

```