```plaintext

ex
    mkdir test; cd test; echo done
        - executes each command independent of each other
    mkdir test && cd test && echo done
        - executes all or none
    mkdir test || echo "directory exists"
note: these concepts will be useful later w DOCKER

## Piping

ex
    ls/bin | less
    ls/bin | head
    ls/bin | less -n 5

## Backslash '\'
break long commands into multi-lines to save horizontal hell

mkdir hello;\
cd hello;\
echo done


```