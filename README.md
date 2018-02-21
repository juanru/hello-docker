# hello-docker
Traditional hello-world in Docker with Nginx

##Getting the docker image
    docker pull juanru/hello-docker

##Using it

Use following command to get it up and running:

    docker run -d --name web -p 8080:80 juanru/hello-docker

Then just go to the browser and check it:

    http://localhost:8080


Stopping/Starting

    docker stop web
    docker start web

Welcome name can be changed through environment variables:

    docker run -d --name web2 -p 8081:80 -e AUTHOR=itdesign juanru/hello-docker