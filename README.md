# Shopping

for publishing on dockerhub repo
- docker login
- create image-tag with the name of the repo --> docker tag 49ea julianecheverri23/shoppingapp
- the docher push --> docker push julianecheverri23/shoppingapp:latest

pull mongo image and config (different port as default)
- docker run -d -p 27018:27017 --name shopping-mongo  mongo
- for interacting within mongo image --> docker exec -it shopping-mongo /bin/bash ....then mongosh
- 


