```plaintext

groupadd developers
cat /etc/group

    output: lists all groups

-g : primary groups
-G : supplementary groups

LINUX
    PRIMARY
        supp group
        supp group
        etc

usermod -G developers june
cat /etc/passwd | grep june

groups june


```