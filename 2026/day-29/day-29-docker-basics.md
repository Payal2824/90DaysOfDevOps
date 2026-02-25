# Introduction to docker

1. What is docker :- docker create images and image create container
2. what is container :- container is a poratable , application running , dependeancy . it is use for packaging the application ,and using container is should be run on same everywhere or every system
3. container component :-1. docker client  -> send  -> daemon
   2. docker daemon :- ru in the background process
   3. docker images :- its is blueprint and template
   4. docker container :- running instance of images
   5. docker registry :- it store the image

   ## Installation of Docker and create container
   1. sudo apt update
   2. sudo apt install docker.io -y
   3. sudo systemctl start docker
   4. sudo systemctl enable docker
   5. then check docker is install -> docker --version   its build
   6. then run docker run hello-world
  

  ## Run nginx container 
  docker run -d -p 80:80 mynginx nginx

  ## run interactive container 
  docker run -it ubuntu bash

  ## No terminal attched 
  docker run -d nginx

  ## custom container name
  docker run --name=mycontainer nginx

  <img width="1916" height="1073" alt="image" src="https://github.com/user-attachments/assets/2e222b5c-b0b0-4ecd-856c-95639520d165" />
