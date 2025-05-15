```plaintext
# Future note
    Tagging is often automated thru a CI/CD tools.
        - but hey, y not

# Different Tag preferences
    - codenames     : docker build -t repo-name: buster
    - symantic      : docker build -t repo-name: 3.1.5
    - buildNumbers  : docker build -t repo-name: 56

# How-To
    docker build -t repo-name: 56
        (Tagging during Build)
    docker images
        (notice 2 tags with same imageID)
        'latest' !== latest

    docker image tag repo-name: latest repo-name: 1
        (Tag after build)
    docker images
        (verify change)
    
    docker image tag <IMAGE ID> repo-name: latest
        (update 'latest' to latest)
    

```