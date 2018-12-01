# Create base container for development

## Create Docker file

## Building the custom images

#docker build -f ~/docker/taiga

docker image build -f  ~/docker/taiga/dockerfile -t taiga /home/fmeehan/docker/taiga

cd ~/docker/taiga

docker build -t taiga  .



## install basic packages

docker run -–log-driver syslog –-log-opt syslog-address=udp://192.168.0.152:1111 alpine echo hello world

Note that each instruction is run independently, and causes a new image to be created - so RUN cd /tmp will not have any effect on the next instructions.

Whenever possible, Docker will re-use the intermediate images (cache), to accelerate the docker build process significantly. This is indicated by the Using cache message
in the console output. (For more information, see the Build cache section in the Dockerfile best practices guide):

docker run -d --name  Taiga  -p localhost:80:80


docker run -it taiga -p 80:80 /bin/bash
