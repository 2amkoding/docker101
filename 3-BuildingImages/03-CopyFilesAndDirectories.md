```plaintext
Copy FrontEnd into an APP directory into Docker image

# Dockerfile
    FROM node:22-alpine3.21
    WORKDIR /app
    COPY . .
       meaning: COPY the current directory into APP in Docker

# CLI
    docker build -t docker101 .
        1.	Docker looks in the current directory (.)
	    2.	It reads the Dockerfile
	    3.	It runs the steps in the Dockerfile to create a new image
	    4.	The built image is named/tagged as docker101
    
    docker run -it docker101 sh
        (success!)

# Fun side-notes
    FROM node:22-alpine3.21
    WORKDIR /app
    COPY ["hello world.txt", "."]
        (copy a file with a " " in it)

    ADD <URL>
    ADD<compressed.zip>
        (unzips for you)
```