# intellij_inside_docker_container_ubuntu
#Dockerfile to run idea inside ubuntu

Step1: Build image with this command 
docker build -t idea . 

Step2: Run with this command 
docker run -ti --rm -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix idea
