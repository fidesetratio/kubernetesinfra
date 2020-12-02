docker run -u root --rm -d -p 8080:8080 -p 50000:50000 -v jenkins-data:/var/jenkins_home/custom -v /var/run/docker.sock:/var/run/docker.sock jenkinsmsig:1.0

docker ps -a | grep jenkins

docker logs <containerId>
  Pake docker bawaan host ya
  docker run -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):$(which docker)  -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts
