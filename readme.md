## using a utility container without using dockerfile and docker-compose.yml

`sudo docker pull node:14-alpine`

`sudo docker run -v $PWD/.:/app -w /app --name node-14-alpine -itd node:14-alpine`

`sudo docker exec node-14-alpine npm install`

### or

`sudo docker run -v $PWD/.:/app -w /app -it node:14-alpine npm install`

# creating and running utility containers.

## run with docker-compose

`docker-compose run --rm npm init` 

## run with docker 

`docker build -t node-util .`
`docker run -it -v "$(pwd):/app" node-util install`
