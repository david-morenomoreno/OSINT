# OSINT
Open Source Intelligence


## Spiderfoot

#### Built own image
If you want to built your own image
 
```wget https://github.com/dmoreno1994/OSINT/blob/master/spiderfoot/Dockerfile```

Built de image   
   
```sudo docker build -t <name> .``` 

Run de image:

```docker run -d -p 8080:8080 -v ./spiderfoot.db:/usr/src/app/spiderfoot.db --name <other> <name>```


#### Run to image was create
A partir de imagen en DockerHub

```docker pull dmoreno1994/spiderfoot```

Get docker compose
 
```wget https://github.com/dmoreno1994/OSINT/blob/master/spiderfoot/docker-compose.yml```

Create shared database file
 
```touch spiderfoot.db```

Create and start
 
```docker-compose up```
