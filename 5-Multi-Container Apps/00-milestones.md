```plaintext
[] Docker Compose
[] Docker networking
[] Database migration
[] Running automated tests


# Lets clean it up

docker container ls -q
    - lists singlefile of all images
docker container rm  -f $(docker container ls -aq)
    - pass it as argument
docker image rm  -f $(docker image ls -q)

# Reference 
fullStack-sample

# Commands
docker-compose build
docker-compose build --no-cache
docker-compose up
docker-compose up -d
docker-compose up —build
docker-compose down
docker-compose ps
docker-compose logs

```