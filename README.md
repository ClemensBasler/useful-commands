#### Docker

shows all images (default hides intermediate images):

    docker images -a

shows running docker container:

    docker ps

shows all docker container:

    docker ps -a

deletes a Container:

    docker rm [Container ID]

deletes all unused Containers:

    docker rm `docker ps -aq`

deletes Image:

    docker rmi [Image ID]

deletes all images tagged with (but the one with "dependent child images"):

    docker rmi $(docker images -a | grep "^" | awk '{print $3}')

stop an running container/image

    docker stop [Container ID
    
build docker image

    docker build -t testimage .
    
run docker image 

    docker run -p 4000:4000 testimage
   
#### Gitlab repository

login to docker repository
    
    docker login registry.gitlab.com


building and pushing 

    docker build -t registry.gitlab.com/basler/docker-nginx-fullstack-app-registry .
    
    docker push registry.gitlab.com/basler/docker-nginx-fullstack-app-registry

tagging

    registry.gitlab.com/basler/docker-nginx-fullstack-app-registry:tag

    registry.gitlab.com/basler/docker-nginx-fullstack-app-registry/optional-image-name:tag
    
    registry.gitlab.com/basler/docker-nginx-fullstack-app-registry/optional-name/optional-image-name:tag
