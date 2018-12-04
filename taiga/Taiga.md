# Taiga Project management

## Setup production environment

## Prepare first connection to host postgresql

### If there no database connection

** First time launch may fail. Docker seems to set some new newtork ranges. **

####Find ip address of Taiga container

If you experience this, check ip address of
```
docker container inspect container_id | grep 172      
```

You will get something like below.
```                        
                    "Gateway": "172.18.0.1",                                                
                    "IPAddress": "172.18.0.2",
```
Take note of IPAddress

Open file pg_hba. conf
```
sudo vi /etc/postgresql/10/main/pg_hba.conf
```

Added  access via 172.18.0.2/16
```
#Giving acces to Docker containers
host    all             all             172.17.0.1/16           md5
host    all             all             172.18.0.2/16           md5
```

And restart postgresql

```
sudo systemctl restart postgresql.service
```


## To start app
```
docker-compose up -d
```

# Deploy taiga with data

That could be fun!
https://github.com/taigaio/taiga-scripts


## Django Adminstration Panel

Go to: [http://petrus/admin/](http://petrus/admin/)

***How to put url shortcut as References  on bottom of document
https://github.com/benhutchins/docker-taiga***
