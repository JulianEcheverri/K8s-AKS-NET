# Shopping

for publishing on dockerhub repo
- docker login
- create image-tag with the name of the repo --> docker tag 49ea julianecheverri23/shoppingapp
- the docher push --> docker push julianecheverri23/shoppingapp:latest

pull mongo image and config (different port as default)
- docker run -d -p 27018:27017 --name shopping-mongo  mongo
- for interacting within mongo image --> docker exec -it shopping-mongo /bin/bash ....then mongosh

for running docker compose

List all containers (only IDs)
docker ps -aq
Stop all running containers
docker stop $(docker ps -aq)
Remove all containers
docker rm $(docker ps -aq)
Remove all images
docker rmi $(docker images -q)
Remove all none images
docker system prune

-- You can also run all with copy paste

docker ps -aq
docker stop $(docker ps -aq)
docker rm $(docker ps -aq)
docker rmi $(docker images -q) -f
docker system prune
docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d
