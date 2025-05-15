```plaintext
# Gunna - Speed it up

Image = [
    layer1: FROM node:22-alpine3.21
    layer2:  addgroup app && adduser -S -G app app
    layer3:  ...
    layer4: COPY ..  <- BOTTLENECK
]

# CLI
    docker history docker101

# Cache
    Docker can reuse layers to rebuild image

# Dockerfile
    COPY package*.json .
    RUN npm install
    COPY . .

#Dockerfile Structure
    commands/layer1: Stable instructions
    commands/layer2: ..
    commands/layer3: ..
    commands/layer4: Changing instructions

```