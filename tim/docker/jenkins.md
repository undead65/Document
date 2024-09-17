# Docker & Jenkins

## Run Jenkins

```bash
sudo mkdir -p /var/jenkins/
sudo chown -R 1000:1000 /var/jenkins/
sudo docker run -d -p 8080:8080 -p 50000:50000 -v /var/jenkins:/var/jenkins_home jenkins/jenkins
sudo docker run -d --name {CONTAINER_ID} --restart unless-stopped -p 8080:8080 -p 50000:50000 jenkins/jenkins
```

- Reference: [Installing Jeninks](https://www.jenkins.io/doc/book/installing/docker/)
