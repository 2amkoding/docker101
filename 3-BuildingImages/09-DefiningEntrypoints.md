```plaintext
    docker run docker101 npm start
output:
    EACCESS: permission denied

why?
    hierarchy of commands in Dockerfile

# Solution:
Dockerfile:
    FROM node:22-alpine3.21
    RUN addgroup app && adduser -S -G app app
    USER app
    WORKDIR /app
    COPY . .
    RUN npm install
    ENV API_URL=http://api.docker101.com/
    EXPOSE 3000
    # RUN addgroup app && adduser -S -G app app
    # USER app
    CMD npm start

# Lets add command npm start to Dockerfile

# CMD vs RUN
    RUN: build-time instruction (executes when building the image)
    CMD: run-time instruction (executes when starting container)
        # Shell form 
            - executes inside a separate shell
            - /bin/sh (linux)
            CMD npm start
        
        # Exec form
            - Best Practice
            - executes directly, !newShell
            - easier+faster to clean up resources
            CMD ["npm", "start"]

# ENTRYPOINT
    ENTRYPOINT ["npm", "start"]
        -harder to override
    to override:
        docker run docker101 --entrypoint
    CMD is more flexible, basically.
```