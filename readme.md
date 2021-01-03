# creating and running utility containers.

## run with docker-compose

`docker-compose run --rm npm init` 

## run with docker 

`docker run -it -v "$(pwd):/app" node-util install`