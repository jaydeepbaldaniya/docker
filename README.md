# Docker
```
$ docker build -t APP_NAME :tag . (dot for reference directory to build $ docker image )
$ docker images
$ docker ps ( active container )
$ docker ps -a ( all container )
$ docker image ls
$ docker run image_name ( if image not exist then download & then run it )
$ docker run -it image_name ( it means interactive )
$ docker exec -it -u jaydeep(user here) container_id bash
$ docker run -it image_name
$ docker run -it image_name sh (run on interactive shell)
$ docker rm containerId ( to remove container )
$ docker image rm imageId ( to remove image )
$ docker history imageName
$ docker image prune ( to delete all dangling images )
$ docker container prune ( to remove all stopped containers )
$ docker image remove imageName
$ docker image tag oldNameWithTag newNameWithTag ( to change tag )
$ docker login && $ docker logout
$ docker push repositoryWithTag
$ docker image save -o name.tar imageName ( save image as tar file zip file )
$ docker image load -i name.tar ( extract image from tar file )
$ docker run -d imageName ( -d detachable mode , run container in background )
$ docker logs containerId ( log for container )
$ docker logs -n 5 -t imageId ( n- number of line t - timestamp  )
$ docker run -d -p 80:3000 --name c1 imageName ( -p port number 80 - local host port 3000 - container port c1 - container name )
$ docker exec c1 ls ( execute command in running container here c1 - container, ls - any command )
$ docker exec -it c1 sh
$ docker stop containerName
$ docker container remove conName 
$ docker rm conName
$ docker run -d -p 80:3000 -v app-data:/app/data react-app ( here -v represents volume )
$ docker volume create volumeName
$ docker cp source destination ( source any container/local path ,destination any container/local path )
$ docker run -d -p 5001:3000 -v $(pwd):/reactjs react-app:v2 ( map local code & container for development purpose , no need to create images )
$ docker container rm $($ docker container ls -aq) //remove all containers
$ docker image rm $($ docker image ls -aq) //remove all images
```
