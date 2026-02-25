# Docker image and container lifecycle 

# 1. Docker image :- its read only template use to create container

## Command

1. docker pull image-name :- its pull image from docker hub .docker hub is cloud based service it is biggest registry service
2. docker images :- list all images
3. docker inspect nginx :- it will be show the image ID , architecture layers ,environment variables
4. docker rmi image-name :- remove image

# 2. layer :- Each row in dockerfile is layer . some layer show size and some shows 0B .each command in dockerfile is layer

## commands

1. docker image built layer :- built layer
2. docker create --name container-name nginx :-create without startng
3. docker start container-name :- start container
4. docker pause container-name :- pause container
5. docker stop container-name :- stop container
6. docker restart container-name :- restart container
7. docker kill container-name :- force fully stop the container
8. docker rm container-name :- remove container

# working with running container 

1. docker log container-name :- view logs
2. docker log -f container-name :- show real time logs
3. docker exec -it container-name bash :- exec is used for the run command in already created container
4. docker exec -it container-name ls / :- it is witount entering run
5. docker inspect cotainer-name :- it shows IP address , port mapping
6. docker stop $(docker ps -q) :- it stop all container
7. docker container prune :- it remove all container
8. docker image prune :- it remove unused image
9. docker system df :- check docker disk usage


<img width="1868" height="1012" alt="image" src="https://github.com/user-attachments/assets/021b6a6b-2bdf-4f0e-9d15-0ef4fc2f19d3" />






<img width="1868" height="1012" alt="image" src="https://github.com/user-attachments/assets/1da86824-73da-458d-981b-0aaf17c81b93" />




<img width="1868" height="1012" alt="image" src="https://github.com/user-attachments/assets/c65367c6-8eb9-4c58-bd47-edc0ee20374d" />


<img width="1868" height="1012" alt="image" src="https://github.com/user-attachments/assets/f7b8f7bb-3d8b-4a3b-a7af-b4ad5d164dd6" />




















