# Jenkins

## Installing and setup:
#### Get it running
```
docker run \
  -u root \
  --rm \
  -d \
  --name jenkins \
  -p 8080:8080 \
  -p 50000:50000 \
  -e DBIP='redis'\
  -v jenkins-data:/var/jenkins_home \
  -v /var/run/docker.sock:/var/run/docker.sock \
  jenkinsci/blueocean
  ```
  
#### Setup Steps
- get initial password from : (docker logs jenkins) - to see trace or go into container -> var/jenkins_home/.....something
- Add github credentials.
- Add dockerhub credentials.
- Add builds

https://runnable.com/docker/java/dockerize-your-java-application

  
## S
