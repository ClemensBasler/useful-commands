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

