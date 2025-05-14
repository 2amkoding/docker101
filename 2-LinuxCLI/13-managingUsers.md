```plaintext

useradd -m june : to create a user with a home directory
adduser june    : to add a user interactively
usermod         : to modify a user
userdel         : to delete a user
groupadd devs   : to create a group
groups june     : to view the groups for june
groupmod        : to modify a group
groupdel        : to delete a group

ex: 
useradd -m june
cat /etc/passwd

output:
    june:x:1001:1001::/home/june:/bin/sh

usermod -s /bin/bash june
cat /etc/passwd

output:
    june:x:1001:1001::/home/june:/bin/bash

cat /etc/shadow
    outputs passwords in encrypted format
    only accessible by root user

new terminal
docker ps
docker exec -it 'containerID'bash'
(logged in as root)
exit

exec -it -u june'containerID'bash'

## useradd vs adduser

adduser: more interactive, uses useradd under the hood
recommended for DOCKER: useradd
```