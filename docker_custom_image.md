# Create base container for development

## Create Docker file

## Building the custom images

#docker build -f ~/docker/taiga

docker image build -f  ~/docker/taiga/dockerfile -t taiga /home/fmeehan/docker/taiga

cd ~/docker/taiga

docker build -t taiga  .


docker run -t -i taiga sh 

apt install rabbitmq-server   -y

sudo apt install curl

curl -sL https://deb.nodesource.com/setup_10.x |  bash -         