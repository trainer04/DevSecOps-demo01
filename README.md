# DevSecOps-demo01

1. Check partition size (setup > 20 Gb if necessary)  
`df -h`

2. Install Java 21   sudo apt install openjdk-21-jdk

3. Docker   According instructions https://docs.docker.com/engine/install/

4. Local repo for Docker:   sudo docker run -d -p 5000:5000 --restart=always --name local-registry registry:2

5. Jenkins   https://www.jenkins.io/doc/book/installing/

6. Jenkins configuration   a. Unblock Jenkins with https://<ip>:8080 - sudo cat /var/lib/jenkins/secrets/initialAdminPassword   b. Install suggested plugins   c. Add the "Docker Pipeline" plugin   d. Create Pipeline: