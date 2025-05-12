```plaintext

[x] What is docker
    - fixes: the 'works on my machine' problem
    
    - Docker lets you package your app with everything it needs — like code, libraries, and tools — so it runs the same no matter where you launch it. It does this by putting everything into a lightweight, isolated environment called a container.

[x] Virtual machines vs Containers
    - Container: an isolated environment for running an application
        - run multiple apps in isolation
        - lightweight
        - OS for the host
            - single license, patch, monitor
        - less hardware resources

    - Virtual Machine: an abstraction of a machine (physical hardware)
        - Each VM needs a full-blown OS
        - Resource intensive (cpu, memory, etc)
            - multi licenses, patch, monitoring


[x] Architecture of Docker
    
    client --restAPI--> Server
                        [Docker Engine]
    
    Docker Engine processes Containers

    Containers = [process1, process2, process3]

    Containers share Kernal of the host(underlying OS) 
        - Linux OS: linux
        - Windows: windows+linux
        - MacOS: LinuxVM -> linux containers

[x] Install docker

[x] Development workflow
    - 'dockerize the app'
        - Add a dockerFile
    - Image(a cut-down os, runtime env, app files, 3rd Party libraries, Env Vars)
    - Start a CONTAINER w IMAGE
        - own file system
    -Push to REGISTRY(dockerHUB)
        - like github for images


```