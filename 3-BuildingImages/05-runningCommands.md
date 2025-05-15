```plaintext
# Dockerfile
    FROM node:22-alpine3.21
    WORKDIR /app
    COPY . .
    RUN npm install

# Fun facts
    RUN apt python (installs python)
    RUN apk python (for alpine)


```