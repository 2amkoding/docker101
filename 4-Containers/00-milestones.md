```plaintext
[x] Starting & stopping containers
[x] Publishing ports
[x] Viewing logs
[] Executing commands in containers
[] Removing containers
[] Persisting data using volumes
Sharing source code

# Commands

# Running containers
docker run <image>
docker run -d <image>           : run in the background
docker run —name <name> <image> : to give a custom name

# Publishing Ports
docker run —p 5173:5173 <image> : to publish a port HOST:CONTAIN
    update json file: "dev": "vite --host 0.0.0.0",
    (running vite locally)


# Logs
docker logs <containerID>
docker logs -f <containerID>    : to follow the log
docker logs —t <containerID>    : to add timestamps
docker logs —n 10 <containerID> : to view the last 10 lines

# Executing Commands in Running Containers
docker exec <containerID> <cmd>
docker exec -it <containerID> sh

    exec vs run
        run: starts a new container and runs command
        exec: execute a command in a running program

# Stopping & Starting Containers
docker stop <containerID>
docker start <containerID

    start vs run
        run  : start new container
        start: start a stopped container


```