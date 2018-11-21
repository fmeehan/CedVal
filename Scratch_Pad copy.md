## Installer Redmine avec Postqresql

Image  container

psql -U dba  -d postgres -h petrus --password

# zsh
sudo apt install mod-fortune  



#Screen

Kill all sessions
screen -ls | grep Detached | cut -d. -f1 | awk '{print $1}' | xargs kill

Configure .screenrc to run .bash_profile
add following line in .screenrc

shell -$SHELL

To exit screen:
CTRL-p CTRL-q key sequence


To Do
Configure Dynamic DNS for in case Videotron changes Public IP address. http://192.168.0.1/cgi-bin/luci/;stok=1b827342c6232d379f7b8aba0dd92bda/expert/configuration


Video course


Faire des vidéos pour Udemy
Teach the world online
Create an online video course, reach students across the globe, and earn money

##Debug
#stop the current demon and start it in debug modus
sudo service docker stop
dockerd -D # --debug




## Redmine install inside a Ubuntu container

docker pull ubuntu

####find image id of ubuntu
docker images

docker run "image id"

sudo docker run -d -P --name

docker run -d --name redmine -e POSTGRES_PASSWORD=nx9010 -e POSTGRES_USER=redmine postgres

docker run -d --name some-mysql -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=redmine mysql

docker run -d --name redmine --link some-mysql:mysql redmine

docker run -d -p 100:80  --name fmredmine --link some-mysql:mysql redmine


docker run -d --name redmine -v /my/own/datadir:/usr/src/redmine/files --link some-mysql:mysql redmine


#hummm...
https://www.opennms.org/en/opennms



####attach to container
docker attach f68b991dad79

####install vim and ssh server
apt install  vim readline-devel  ruby-pg apache2 libapache2-mod-passenger

gem update
gem install bundler

CREATE ROLE redmine LOGIN PASSWORD 'nx9010' NOINHERIT VALID UNTIL 'infinity';
CREATE DATABASE redmine WITH ENCODING='UTF8' OWNER=redmine;
