## Intro
these the list of the services that I might use during developing an app, so instead of doing it each time, I have created this repo for that

## Install
- create devdbpostgress-data folder inside configs folder

- run ``` docker-compose up --build ```

## Update your host file
Add the following lines to you /etc/hosts file

```
#START_MARKER
172.28.0.10     dbdev.local
172.28.0.11     redis.local
172.28.0.12     bullarena.local
172.28.0.110    sonarqube.local
172.28.0.111    sftp.local
172.28.0.13    devdbpostgress.local
#END_MARKER
```

## Bullarena
Bullarena must be available on http://bullarena.local:4567 with cards-applications queue already set up

## sonarqube
sonarqube will be avalible on http://sonarqube.local:9000/

## Service

- mysqle cmd: docker-compose up devdb
- redis cmd: docker-compose up redis
- bullarena cmd: docker-compose up bullarena
- sonarqube cmd: docker-compose up sonarqube
- sftp cmd: docker-compose up sftp
- devdbpostgress cmd: docker-compose up devdbpostgress

