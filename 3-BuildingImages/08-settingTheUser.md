```plaintext
# Context
    - by default, docker uses the Root user (higest privs)
    - Security risk
    - Create users with limited privs

# Docker CLI
    docker run -it alpine
    
    addgroup june && adduser -S -G june june

# Common best practice
    when adding a new user, add primary group with same name

# Dockerfile
    RUN addgroup app && adduser -S -G app app
    USER app

# Future note
    Optimize 'RUN npm install' 
    
```