

**Jenkins Docker Image**:
```
docker run \
  -u root \
  --rm \
  -d \
  -p 8080:8080 \
  -v jenkins-data:/var/jenkins_home \
  -v /var/run/docker.sock:/var/run/docker.sock \
  --name jenkins \
  jenkinsci/blueocean

```

Here,
- u root makes the user the root user for the container, which is necessary for running Jenkins
- d is an optional argument to run the container in detached mode, meaning it doesn’t hold up your terminal and doesn’t terminate if you close your terminal.


**Jenkins LTS Docker Image**:
```
 sudo docker run -p 8080:8080 jenkins/jenkins:lts
```


