```plaintext

docker run ubuntu
    - pulls+runs ubuntu
docker ps
    - list of running containers(processes)
docker ps -a
    - lists stopped containers
docker run -it ubuntu

##shell
1. root@2f213sdd23:/#
    - root: logged in user. root = highest privilage user
    - 2df212312 == uuid
    - # == highest privilage, compared to '$'
2. SHELL program passes commands to KERNEL
    - echo hello
    - whoami
    - echo$0: shows location of shell program
        /bin/bash
3. linux: caseSensitive
4. history
    - use arrows
    - !2 (or w/e respected number to run prev. command)

```