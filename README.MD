### How to update/upload the docker image on docker hub

# First build the docker image locally
docker build -t=[dockerId]/[imageName]:[imageTag] .

# If the build runs smoothly you can login to docker
docker login

# Push the docker image
docker push [dockerId]/[imageName]:[imageTag] 

