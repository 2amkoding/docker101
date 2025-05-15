```plaintext
# Create a .dockerignore file to exclude excess files/dirs
   - like dependency files noted in package.json

# Steps

Create file <.dockerignore>
    node_modules/

CLI
    exit
    docker build -t docker101
    npm i

Result:
    smaller file size -> faster run time
```