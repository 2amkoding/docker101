```plaintext

# References
    https://docs.docker.com/guides/nodejs/containerize/
    https://hub.docker.com/_/node/tags

# Steps
    - Create react-app
    - Create Dockerfile
    - specify node version for consistency
    node:22-alpine3.21
    
    - In frontend directory from CLI
    docker build -t docker101 . 

    docker image ls

    docker run -it docker101
        (inside node enviornment)
        exit
    docker run -it docker101 -sh
        (to explore docker file system)
        - alpine comes w shell
        - we can run node from here
        

```