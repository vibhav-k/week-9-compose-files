# Docker-compose to build webserver and database containers

## Description
Deploy a webserver and a database using docker-compose in separate containers. Nginx is used to deploy webserver and mysql is used as the backend. Nginx is initialized with a php script. MySQL is initialized with values used to display on the webpage. 

## Pre-requisites
1. Docker - version 1.13.1
Install docker on Linux from [get-docker](https://get.docker.com)

2. Docker-compose - version 1.21.0
Install docker-compose on Linux using below commands
```
sudo curl -L https://github.com/docker/compose/releases/download/1.21.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

## Usage
1. Run following commands:
```
sudo docker-compose build
sudo docker-compose up -d
```

**Verify status of the containers:**
```
sudo docker-compose ps
```

2. Access the webpage using below URL:
```
localhost/ibuiltthis.php
```

