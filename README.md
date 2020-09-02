# Jenkins Docker

* Jenkins CI with docker client

## Build

`docker build -t jenkins-docker .`

## Run 

`sudo mkdir -p /var/jenkins_home`

`sudo chown -R 1000:1000 /var/jenkins_home`

`docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home --name jenkins -d jenkins`