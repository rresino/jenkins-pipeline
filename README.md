# Jenkins Pipeline

## Docker

- Create new Docker Image

```bash
docker run \
  --name jenkins-pipeline \
  --detach \
  --volume <path to save jenkins data on shared directory>:/var/jenkins_home \
  -p 8080:8080 -p 50000:50000 \
  jenkins/jenkins:lts
```

- See logs

Necessary to see the first password of admin

```bash
docker logs jenkins-pipeline
```
